# Hexalith Template Package

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A template repository for creating new .NET packages within the Hexalith ecosystem. This template provides a standardized structure and configuration for developing, testing, and publishing packages that adhere to Hexalith's coding standards and practices.

## Features

- Standardized project structure for source code and tests
- Centralized build configuration through the Hexalith.Builds submodule
- Consistent code style and analysis rules
- Integrated CI/CD workflows for building, testing, and publishing packages
- Centralized package version management

## Getting Started

### Prerequisites

- .NET SDK (version specified in `Hexalith.Builds/Framework.Build.props`)
- Git
- Visual Studio, Visual Studio Code, or another compatible IDE

### Quick Start

1. Create a new repository using this template
2. Clone the repository to your local machine
3. Initialize and update the Hexalith.Builds submodule:

```powershell
git submodule update --init --recursive
```

Alternatively, you can use the provided script:

```powershell
.\Hexalith.Builds\Tools\builds-submodule-init.ps1
```

4. Rename the solution and projects to match your package name
5. Start developing your package in the `src/` directory
6. Add tests in the `test/` directory

## Repository Structure

```
Hexalith.Template.Package/
├── .github/                  # GitHub workflows and configuration
├── Hexalith.Builds/          # Submodule containing build configurations
├── src/                      # Source code for package projects
├── test/                     # Test projects
├── .gitignore                # Git ignore file
├── .gitmodules               # Git submodules configuration
├── LICENSE                   # License file
└── README.md                 # This file
```

## Build System

This template uses the Hexalith.Builds submodule for build configuration. For more information, see the [Hexalith.Builds README](Hexalith.Builds/README.md).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.