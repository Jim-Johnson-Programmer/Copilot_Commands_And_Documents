# Updating and Configuring .NET Projects

This guide covers common procedures for setting up, updating, and configuring .NET projects, including referencing other projects, managing NuGet packages, and ensuring version consistency.

---

## 1. Adding Project References

**Copilot Command:**  
```plaintext
/addProjectReference MyApp/MyApp.csproj ../MyLibrary/MyLibrary.csproj
```
**Manual Command:**  
```plaintext
dotnet add <target_project> reference <path_to_project_to_reference>
```
**Example:**
```plaintext
dotnet add MyApp/MyApp.csproj reference ../MyLibrary/MyLibrary.csproj
```

---

## 2. Adding NuGet Packages

### Add the Latest Version of a Package

**Copilot Command:**  
```plaintext
/addNugetPackage MyApp Newtonsoft.Json
```

**Manual Command:**  
```plaintext
dotnet add <project> package <package_name>
```
**Example:**
```plaintext
dotnet add MyApp package Newtonsoft.Json
```

### Add a Specific Version of a Package

**Copilot Command:**  
```plaintext
/addNugetPackage MyApp Newtonsoft.Json 13.0.3
```

**Manual Command:**  
```plaintext
dotnet add <project> package <package_name> --version <version>
```
**Example:**
```plaintext
dotnet add MyApp package Newtonsoft.Json --version 13.0.3
```

---

## 3. Matching Package Version to Another Project

**Copilot Command:**  
```plaintext
/matchNugetVersion MyApp Serilog MyLibrary
```

**Manual Steps:**  
- Open the `.csproj` file of the reference project and find the `<PackageReference>` entry.

**Manual Command:**  
```plaintext
dotnet add <project> package <package_name> --version <version_from_other_project>
```
**Example:**
```plaintext
dotnet add MyApp package Serilog --version 2.12.0
```

---

## 4. Updating All Packages to Latest

**Copilot Command:**  
```plaintext
/updateAllNugetPackages MyApp
```

**Manual Command:**  
```plaintext
dotnet outdated --upgrade
```
> Requires [dotnet-outdated tool](https://github.com/dotnet-outdated/dotnet-outdated).

---

## 5. Restore Packages

**Copilot Command:**  
```plaintext
/restoreNugetPackages MyApp
```

**Manual Command:**  
```plaintext
dotnet restore
```

---

## 6. Remove a NuGet Package

**Copilot Command:**  
```plaintext
/removeNugetPackage MyApp Newtonsoft.Json
```

**Manual Command:**  
```plaintext
dotnet remove <project> package <package_name>
```
**Example:**
```plaintext
dotnet remove MyApp package Newtonsoft.Json
```

---

## 7. Change Target Framework

**Copilot Command:**  
```plaintext
/setTargetFramework MyApp net8.0
```

**Manual Edit:**  
Edit the `<TargetFramework>` in the `.csproj` file:
```xml
<PropertyGroup>
  <TargetFramework>net8.0</TargetFramework>
</PropertyGroup>
```

---

## 8. Useful References

- [dotnet CLI documentation](https://learn.microsoft.com/dotnet/core/tools/)
- [NuGet CLI documentation](https://learn.microsoft.com/nuget/tools/nuget-exe-cli-reference)
- [dotnet-outdated tool](https://github.com/dotnet-outdated/dotnet-outdated)

---
"Change the target framework of MyApp to .NET 8.0."

**Situation 2: Copilot Command**  
```plaintext
/setTargetFramework MyApp net8.0
```

**Manual Edit:**  
Edit the `<TargetFramework>` in the `.csproj` file:
```xml
<PropertyGroup>
  <TargetFramework>net8.0</TargetFramework>
</PropertyGroup>
```

---

## 9. Adding and Configuring Groups of NuGet Packages

You can add related NuGet packages as a group (e.g., Entity Framework Core, Serilog) and have Copilot configure them in your `Program.cs` automatically.

### Example: Add and Configure Entity Framework Core

**Copilot Command:**  
```plaintext
/addNugetGroup MyApp efcore
```
_Copilot will add the latest Entity Framework Core packages (Microsoft.EntityFrameworkCore, Microsoft.EntityFrameworkCore.SqlServer, etc.) and update `Program.cs` to configure the DbContext._

### Example: Add and Configure Serilog

**Copilot Command:**  
```plaintext
/addNugetGroup MyApp serilog
```
_Copilot will add Serilog packages (Serilog, Serilog.AspNetCore, etc.) and update `Program.cs` to configure Serilog as the logging provider._

### Manual Steps

1. **Add all required packages:**
    ```plaintext
    dotnet add MyApp package Microsoft.EntityFrameworkCore
    dotnet add MyApp package Microsoft.EntityFrameworkCore.SqlServer
    dotnet add MyApp package Serilog
    dotnet add MyApp package Serilog.AspNetCore
    ```
2. **Update `Program.cs` to configure the services.**

**Entity Framework Example:**
```csharp
// ...existing code...
builder.Services.AddDbContext<MyDbContext>(options =>
    options.UseSqlServer(builder.Configuration.GetConnectionString("DefaultConnection")));
// ...existing code...
```

**Serilog Example:**
```csharp
// ...existing code...
using Serilog;

Log.Logger = new LoggerConfiguration()
    .WriteTo.Console()
    .CreateLogger();

builder.Host.UseSerilog();
// ...existing code...
```

### How to Get Copilot to Configure Entity Framework in Program.cs

To have Copilot automatically configure Entity Framework Core in your `Program.cs` with a database connection string, use a command like:

**Copilot Command:**  
```plaintext
/configureEfCoreDbContext MyApp MyDbContext "DefaultConnection"
```

- `MyApp` is your project name.
- `MyDbContext` is the name of your DbContext class.
- `"DefaultConnection"` is the name of the connection string in your `appsettings.json`.

_Copilot will add the necessary `AddDbContext` code to `Program.cs` using the specified connection string._

**Resulting code in `Program.cs`:**
```csharp
// ...existing code...
builder.Services.AddDbContext<MyDbContext>(options =>
    options.UseSqlServer(builder.Configuration.GetConnectionString("DefaultConnection")));
// ...existing code...
```

---

## 8. Useful References

- [dotnet CLI documentation](https://learn.microsoft.com/dotnet/core/tools/)
- [NuGet CLI documentation](https://learn.microsoft.com/nuget/tools/nuget-exe-cli-reference)
- [dotnet-outdated tool](https://github.com/dotnet-outdated/dotnet-outdated)

---
