# Contributing to Ubivera Projects

> **Note:** By contributing to projects on the Ubivera organization, you agree to be bound by the [Ubivera Source-Available License v1.0](./LICENSE.md) and the applicable [Contributor Agreement](#contributor-agreement).

## Prerequisites

Before contributing:

- Familiarize yourself with the [Development Guidelines](./Policies/DEVELOPMENT_GUIDELINES.md)
- If you're contributing significant code, please ensure you have signed the appropriate [Contributor Agreement](#contributor-agreement)

---

## Contribution Workflow

1. **Fork** the repository
2. **Create a branch** for your contribution (`feature/my-enhancement`)
3. Write **modular, testable code** following Clean Architecture principles
4. Add or update **unit and integration tests**
5. Run `dotnet test` or `npm test` and ensure **all tests pass**
6. Commit with a **signed commit** (`git commit -S`)
7. **Open a pull request** to the `main` or appropriate working branch

All PRs will be reviewed for:

- Code quality and test coverage
- Architectural alignment
- Security and compliance concerns
- Adherence to the development guidelines

---

## Commit Requirements

- Commits **must be signed**
- Use clear, descriptive commit messages (e.g., `Add JWT validation to API`)
- No credentials, API keys, or secrets in commits or diffs
- Only include changes relevant to the scope of your PR

---

## Contributor Agreement

All contributors must accept and abide by the Contributor Agreement prior to submission. There are two types:

1. **Named Agreement**: If you are explicitly listed, no further action is required.
2. **General CLA**: All other contributors agree to the terms in the generic [Contributor Agreement](./Agreements/CONTRIBUTOR_AGREEMENT.md) by their first pull request.

_By submitting a pull request, you agree to assign all IP in your contribution to Ubivera and affirm that you have the rights to submit the code._

If you have questions about the CLA, contact us at: **legal@ubivera.com**

---

## Security and Dependency Guidelines

- Only use libraries licensed under **MIT**, **Apache 2.0**, or **BSD-3-Clause**
- Do **not** use GPL, AGPL, SSPL, or other copyleft dependencies
- Dependencies must be added via NuGet/npm and declared in the project’s `NOTICE.md`

---

## Code of Conduct

While not yet formalized, we expect all contributors to interact with professionalism, respect, and a shared passion for excellence.