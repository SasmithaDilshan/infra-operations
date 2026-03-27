# infra-operations

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)

infra-operations is a collection of open-source, configurable tools used for infrastructural operations.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [Issue Reporting](#issue-reporting)
- [License](#license)

---

## Overview

infra-operations provides a suite of tools designed to automate, monitor, and manage infrastructure tasks. The project is built with configurability in mind, allowing teams to adapt each tool to their specific environment without significant custom code.

## Features

- **Configurable tooling** – Each tool exposes configuration options so it can be tailored to different infrastructure setups.
- **Open-source** – Licensed under Apache 2.0, free to use and modify.
- **Extensible** – New operational tools can be added following the established project conventions.

## Prerequisites

Before you begin, ensure you have the following installed:

| Requirement | Version  |
|-------------|----------|
| Java (JDK)  | 11+      |
| Maven       | 3.6+     |
| Git         | 2.x+     |

## Getting Started

1. **Clone the repository**

   ```bash
   git clone https://github.com/SasmithaDilshan/infra-operations.git
   cd infra-operations
   ```

2. **Checkout the dev branch**

   ```bash
   git checkout dev
   ```

3. **Build the project**

   ```bash
   mvn clean install
   ```

4. **Run a tool**

   Each tool resides in its own sub-module. Navigate to the relevant module directory and follow its specific README for usage instructions.

## Project Structure

```
infra-operations/
├── LICENSE                  # Apache 2.0 license
├── README.md                # Project documentation (this file)
├── issue_template.md        # Template for filing GitHub issues
└── pull_request_template.md # Template for raising pull requests
```

> As new tools are added, they will appear as sub-directories (Maven modules) inside this root.

## Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for the full contribution guidelines, including:

- How to fork and set up your development environment
- Coding standards and commit message conventions
- How to submit a pull request

When raising a PR, use the provided [pull request template](pull_request_template.md) so reviewers have all the context they need.

## Issue Reporting

If you encounter a bug or have a feature request, open an issue using the [issue template](issue_template.md). Include as much detail as possible (steps to reproduce, affected version, environment details) to help the team triage quickly.

## License

This project is licensed under the **Apache License, Version 2.0**. See [LICENSE](LICENSE) for the full text.

