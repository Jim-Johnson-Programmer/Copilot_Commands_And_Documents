To generate a C# API project using Clean Architecture with Copilot, you'd typically use a starter template or scaffolding tool that supports that structure. While Copilot itself doesn’t have a direct CLI command like `copilot new clean-arch`, you can combine its intelligence with existing tooling like .NET CLI or popular GitHub templates.

Here’s how you can get started quickly:

---

### 🧱 Recommended Clean Architecture Template

Use this GitHub starter: [`jasontaylordev/CleanArchitecture`](https://github.com/jasontaylordev/CleanArchitecture). It includes:

- ✅ ASP.NET Core Web API with CQRS and MediatR
- ✅ Layered separation: `Core`, `Application`, `Infrastructure`, `Web`
- ✅ Integrated DI, testing, validation, logging, and EF Core

---

### ⚡ CLI-Based Setup Steps

```bash
dotnet new install CleanArchitecture.Template
dotnet new cleanarchitecture --name MyProject
```

This creates a fully scaffolded Clean Architecture solution.

---

### 🧠 Copilot Command-Like Prompts You Can Use in VS Code or Copilot Chat

Once your project is set up, try prompts like these:

- “Generate a C# controller for managing products using MediatR and FluentValidation.”
- “Write an Application service for user registration with email validation.”
- “Add T-SQL migration scripts for the Orders table using EF Core.”
- “Refactor my Infrastructure layer to support PostgreSQL instead of SQL Server.”

---

Would you like me to break down the folder structure or recommend how to integrate Angular into the front end? I could also show you how to align this with App Insights or other tools you're using.
