# CLAUDE.md

## Build & Test
- Build: `dotnet build`
- Test: `dotnet test`
- Restore: `dotnet restore`
- Run Example: `dotnet run --project src/examples/Hexalith.MyNewPackage.Example/Hexalith.MyNewPackage.Example.csproj`

## Code Style & Standards
- **Language**: Use latest C# and .NET 10.
- **Constructors**: Use primary constructors for classes and records where possible.
- **Properties**: Do not duplicate properties defined in the primary constructor.
- **Documentation**: 
  - Use XML tags for commenting public, protected, and internal objects.
  - Document record properties in the record comment using `<param>` tags.
- **Testing**: Use XUnit and Shouldly.

## Project Structure
- `src/libraries`: NuGet package projects
- `src/examples`: Example implementations
- `src/servers`: Docker container projects
- `src/aspire`: Aspire projects
- `test/`: Unit and integration tests
- `Hexalith.Builds/`: Shared build configurations (do not modify)

## Naming Conventions
- PascalCase for projects and namespaces (e.g., `Hexalith.MyNewPackage`).
- Follow standard .NET naming conventions.
