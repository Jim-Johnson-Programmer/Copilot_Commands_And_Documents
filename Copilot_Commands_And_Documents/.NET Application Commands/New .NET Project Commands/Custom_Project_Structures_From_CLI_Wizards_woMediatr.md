Absolutely, Jim — you're not alone in preferring a more direct approach. While MediatR is popular for implementing CQRS, it’s not a requirement for Clean Architecture. There are several templates and strategies that stick to the core principles without introducing that extra abstraction.

---

### 🧰 Clean Architecture Templates Without MediatR

Here are a few solid options:

#### 1. **[Ardalis/CleanArchitecture](https://github.com/ardalis/CleanArchitecture)**
- Created by Steve Smith (aka Ardalis)
- Uses FastEndpoints by default, but you can easily swap in controllers or Razor Pages
- No MediatR dependency unless you choose to add it
- Install via CLI:
  ```bash
  dotnet new install Ardalis.CleanArchitecture.Template
  dotnet new clean-arch -o YourProjectName
  ```

#### 2. **[JrDev’s Minimal API Clean Architecture](https://jrdev.io/posts/A-Framework-Without-MediatR/)**
- Focuses on **direct DI** and **minimal APIs**
- No MediatR, no ceremony — just clean layering and explicit service calls
- Great for architectural katas or lean production apps

#### 3. **Custom Service-Based Approach**
- You can fork Jason Taylor’s template and replace MediatR with your own service interfaces
- Example discussion: [Using Services instead of MediatR](https://github.com/jasontaylordev/CleanArchitecture/discussions/814)
- Services like `IToDoListService` can live in the Application layer and be injected directly

---

### 🧠 Why Skip MediatR?

- Avoids extra boilerplate (requests, handlers, etc.)
- Keeps flow traceable and easier to debug
- Reduces third-party dependencies — especially useful in regulated or legacy environments

---

Would you like a walkthrough of how to refactor an existing MediatR-based template to use services or direct DI? I can also help you wire up validation and error handling without losing structure.

You can explore the full structure and NuGet dependencies of the **CleanArchitecture.Template** by visiting the official GitHub repository: [ardalis/CleanArchitecture](https://github.com/ardalis/CleanArchitecture). It’s a well-maintained starter for ASP.NET Core 9 projects following Clean Architecture principles.

---

### 📁 Project Structure Overview

Once generated, the solution typically includes:

- `src/`
  - `Core/` – Domain models, interfaces, and business logic
  - `UseCases/` – Feature-based commands and queries (CQRS style)
  - `Infrastructure/` – Data access, external services, EF Core setup
  - `Web/` – API endpoints using FastEndpoints (can be swapped for controllers)
- `tests/`
  - Unit and integration tests for each layer
- `.template.config/` – Template metadata
- `global.json` – SDK version pinning
- `nuget.config` – Custom NuGet sources if needed

---

### 📦 NuGet Packages Used

Here are the key packages included by default:

| Package               | Purpose                                      |
|----------------------|----------------------------------------------|
| `FastEndpoints`      | Minimal API endpoint abstraction             |
| `FluentValidation`   | Validation logic for requests and models     |
| `AutoMapper`         | Object-to-object mapping                     |
| `MediatR`            | Optional CQRS messaging (can be removed)     |
| `EntityFrameworkCore`| Data access and migrations                   |
| `Ardalis.SharedKernel` | Common base types and abstractions         |
| `NUnit`, `Moq`, `FluentAssertions` | Testing frameworks             |

You can view the full list in the [NuGet Gallery listing](https://www.nuget.org/packages/Clean.Architecture.Solution.Template) or directly in the repo’s `Directory.Packages.props` file.

---

Would you like help customizing this template to remove MediatR and use direct service injection instead? I can walk you through that refactor or even sketch out a sample feature.
