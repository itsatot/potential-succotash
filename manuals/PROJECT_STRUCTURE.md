# Project Structure

This document provides a comprehensive overview of the directory structure for the `nodejs-project-template` repository. It outlines the purpose and organization of each directory and file, ensuring a clear understanding of where to find various components of the project.

## Table of Contents

- [Project Structure](#project-structure)
  - [Table of Contents](#table-of-contents)
  - [./ Directory Layout](#-directory-layout)
  - [./.envs Directory Layout](#envs-directory-layout)
  - [./.github Directory Layout](#github-directory-layout)
  - [./coverage Directory Layout](#coverage-directory-layout)
  - [./dist Directory Layout](#dist-directory-layout)
  - [./docs Directory Layout](#docs-directory-layout)
  - [./manual Directory Layout](#manual-directory-layout)
  - [./src Directory Layout](#src-directory-layout)
  - [./src/enums Directory Layout](#srcenums-directory-layout)
  - [./src/interfaces Directory Layout](#srcinterfaces-directory-layout)
  - [./src/models Directory Layout](#srcmodels-directory-layout)
  - [./tests Directory Layout](#tests-directory-layout)
  - [./tests/enums Directory Layout](#testsenums-directory-layout)
  - [./tests/interfaces Directory Layout](#testsinterfaces-directory-layout)
  - [./tests/mocks Directory Layout](#testsmocks-directory-layout)
  - [./tests/models Directory Layout](#testsmodels-directory-layout)

## ./ Directory Layout

```bash
├── /.envs                                    # Environment configuration files for different environments
├── /.github                                  # GitHub configuration files for commits, issues, and PR templates
├── /coverage                                 # Test coverage reports generated after running the test suite
├── /dist                                     # Compiled output files generated by TypeScript for distribution
├── /docs                                     # Documentation and guides for the project
├── /manuals                                  # Documentation and guides for the project
├── /src                                      # Source code for the CasinoJs library
├── /tests                                    # Unit tests for verifying poker models and project functionality
├── .gitignore                                # Specifies files and directories ignored by Git
├── jest.config.js                            # Configuration file for Jest, defining paths and options for testing
├── LICENSE                                   # License file outlining the terms of distribution
├── package-lock.json                         # Dependency tree capture for consistent installations
├── package.json                              # Project metadata, including dependencies and scripts
├── README.md                                 # Overview of the project, with setup and usage information
├── tsconfig.cjs.json                         # TypeScript configuration for CommonJS builds
├── tsconfig.esm.json                         # TypeScript configuration for ESModule builds
├── tsconfig.json                             # Main TypeScript configuration for overall compiler options
└── typedoc.json                              # Main TypeDoc configuration for overall doc generator options
```

## ./.envs Directory Layout

```bash
├── .env.development.local.example        # Development environment configuration file example
├── .env.example                          # General local development configuration file example
├── .env.local.example                    # Local overrides configuration file example (machine-specific)
├── .env.production.local.example         # Production deployment configuration file example
└── .env.test.local.example               # Test environment configuration file example
```

## ./.github Directory Layout

```bash
├── /COMMIT_TEMPLATE                      # Template for consistent commit messages
│   └── commit_template.md                # Template for TypeScript-related changes (e.g., refactor to TypeScript)
├── /ISSUE_TEMPLATE                       # Templates for GitHub issues
│   ├── bug_report_form.yml               # Updated to include TypeScript-related bug descriptions
│   ├── bug_report_template.md            # Bug reporting template for TypeScript issues
│   └── feature_request_template.md       # Feature request template for new TypeScript features
└── /PULL_REQUEST_TEMPLATE                # Templates for submitting PRs
    └── pull_request_template.md          # Template with TypeScript-related sections
```

## ./coverage Directory Layout

```bash
├── /Icov-report                          # HTML-based coverage reports directory
│   ├── /enums                            # Coverage for enums in the project
│   ├── /models                           # Coverage for models in the project
│   ├── base.css                          # CSS styling for coverage reports
│   ├── block-navigation.js               # JavaScript for navigation within the report
│   ├── favicon.png                       # Favicon for the report HTML pages
│   ├── index.html                        # Main entry point for the coverage report
│   ├── prettify.css                      # CSS for code snippet formatting
│   ├── prettify.js                       # JavaScript for syntax highlighting
│   ├── sort-arrow-sprite.png             # Arrow sprite used in report navigation
│   └── sorter.js                         # JavaScript for sorting report data
│
├── clover.xml                            # XML format report for coverage analysis tools
├── coverage-final.json                   # JSON summary of coverage results
└── lcov.info                             # LCOV format coverage report for tools like Coveralls
```

## ./dist Directory Layout

```bash
├── /cjs                                  # CommonJS entry point after TypeScript compilation
│   ├── enums/                            # Compiled enums for CommonJS
│   ├── interfaces/                       # Compiled interfaces for CommonJS
│   ├── models/                           # Compiled models for CommonJS
│   ├── index.d.ts                        # TypeScript declaration for CommonJS entry point
│   ├── index.js                          # CommonJS entry point after compilation
│   └── index.js.map                      # Source map for CommonJS entry point
│
└── /esm                                  # ESModule entry point after TypeScript compilation
    ├── enums/                            # Compiled enums for ESModule
    ├── interfaces/                       # Compiled interfaces for ESModule
    ├── models/                           # Compiled models for ESModule
    ├── index.d.ts                        # TypeScript declaration for ESModule entry point
    ├── index.js                          # ESModule entry point after compilation
    └── index.js.map                      # Source map for ESModule entry point
```

## ./docs Directory Layout

```bash
├── assets/                           # Static assets for the documentation site
├── classes/                          # Documentation for classes in the project
├── enums/                            # Documentation for enums in the project
├── interfaces/                       # Documentation for interfaces in the project
├── media/                            # Media files like images and diagrams
├── modules/                          # Categorized documentation for modules
├── .nojekyll                         # Prevents GitHub Pages from processing with Jekyll
├── hierarchy.html                    # Project structure in hierarchical format
├── index.html                        # Main entry for the documentation site
└── modules.html                      # List of modules documented within the site
```

## ./manual Directory Layout

```bash
├── CHANGELOG.md                          # Record of changes, updates, and version history
├── CONTRIBUTING.md                       # Guidelines for contributing to the project
└── PROJECT_STRUCTURE.md                  # Detailed explanation of the project directory structure
```

## ./src Directory Layout

```bash
├── /enums                                # TypeScript enums for various poker game-related entities
├── /interfaces                           # TypeScript interfaces for poker game entities defining structures
├── /models                               # Core poker models and logic implementations for the game mechanics
└── index.ts                              # Main export for all modules in the src directory
```

## ./src/enums Directory Layout

```bash
└── index.ts                          # Main export for all enums in the project
```

## ./src/interfaces Directory Layout

```bash
└── index.ts                          # Main export for all interfaces in the project
```

## ./src/models Directory Layout

```bash
└── index.ts                          # Main export for all models in the project
```

## ./tests Directory Layout

```bash
├── /enums                            # Unit tests for enums
├── /interfaces                       # Unit tests for interfaces
├── /mocks                            # Unit tests for mocks
├── /models                           # Unit tests for models
└── index.test.ts                     # Main test file exporting all test modules
```

## ./tests/enums Directory Layout

```bash
└── index.test.ts                     # Aggregated export for all enums in the project
```

## ./tests/interfaces Directory Layout

```bash
└── index.test.ts                     # Main export for all interfaces in the project
```

## ./tests/mocks Directory Layout

```bash
└── index.test.ts                     # Main export for all models in the project
```

## ./tests/models Directory Layout

```bash
└── index.test.ts                     # Main export for all models in the project
```