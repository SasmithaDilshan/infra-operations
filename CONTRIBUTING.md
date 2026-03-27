# Contributing to infra-operations

Thank you for your interest in contributing to infra-operations! We welcome contributions of all kinds — bug reports, feature requests, documentation improvements, and code changes.

---

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How to Contribute](#how-to-contribute)
  - [Reporting Bugs](#reporting-bugs)
  - [Requesting Features](#requesting-features)
  - [Submitting Code Changes](#submitting-code-changes)
- [Development Setup](#development-setup)
- [Coding Standards](#coding-standards)
- [Commit Message Conventions](#commit-message-conventions)
- [Pull Request Process](#pull-request-process)
- [License](#license)

---

## Code of Conduct

Please be respectful and considerate when interacting with other contributors. We are committed to providing a welcoming and inclusive environment for everyone.

---

## How to Contribute

### Reporting Bugs

1. Check the [existing issues](https://github.com/SasmithaDilshan/infra-operations/issues) to see whether the bug has already been reported.
2. If not, open a new issue using the [issue template](issue_template.md).
3. Provide a clear title, a detailed description, steps to reproduce, and information about your environment.

### Requesting Features

1. Search the [existing issues](https://github.com/SasmithaDilshan/infra-operations/issues) for similar requests.
2. If none exist, open a new issue with `[Feature Request]` in the title and describe the use case and expected behaviour.

### Submitting Code Changes

For code contributions, follow the steps in the [Development Setup](#development-setup) section and then submit a pull request as described in [Pull Request Process](#pull-request-process).

---

## Development Setup

1. **Fork** the repository on GitHub.

2. **Clone** your fork locally:

   ```bash
   git clone https://github.com/<your-username>/infra-operations.git
   cd infra-operations
   ```

3. **Add the upstream remote** so you can keep your fork up to date:

   ```bash
   git remote add upstream https://github.com/SasmithaDilshan/infra-operations.git
   ```

4. **Create a feature branch** from `dev`:

   ```bash
   git checkout dev
   git pull upstream dev
   git checkout -b feature/<short-description>
   ```

5. **Build the project** to verify your environment:

   ```bash
   mvn clean install
   ```

---

## Coding Standards

- Follow standard Java coding conventions (Oracle Java Code Conventions).
- Keep methods short and focused on a single responsibility.
- Write Javadoc for all public classes and methods.
- Ensure new code is covered by unit tests where applicable.
- Avoid introducing unnecessary dependencies.

---

## Commit Message Conventions

Use the following format for commit messages:

```
<type>: <short summary>

<optional body – explain why, not what>
```

**Types:**

| Type       | When to use                              |
|------------|------------------------------------------|
| `feat`     | A new feature                            |
| `fix`      | A bug fix                                |
| `docs`     | Documentation changes only               |
| `refactor` | Code change that neither fixes nor adds  |
| `test`     | Adding or updating tests                 |
| `chore`    | Build process or tooling changes         |

**Example:**

```
feat: add disk-usage monitoring tool

Adds a configurable tool for monitoring disk usage across multiple
mount points and emitting alerts when thresholds are exceeded.
```

---

## Pull Request Process

1. Ensure your branch is up to date with `upstream/dev` before opening a PR:

   ```bash
   git fetch upstream
   git rebase upstream/dev
   ```

2. Open the pull request against the `dev` branch (not `main`).

3. Fill in every section of the [pull request template](pull_request_template.md).

4. At least one maintainer must review and approve the PR before it is merged.

5. Address all review comments. Once approved, a maintainer will merge your PR.

---

## License

By contributing, you agree that your contributions will be licensed under the [Apache License 2.0](LICENSE).
