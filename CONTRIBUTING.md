# Contributing to FocusView

**English** | [简体中文](README.zh-CN.md)

Thank you for your interest in contributing to FocusView. This project is a public paradigm, and community participation is essential to its supervision and evolution.

## Code of Conduct

By participating, you agree to maintain a respectful, constructive environment. Focus on the paradigm's public mission: safety, transparency, and user empowerment.

## Development Setup

*(Implementation is in the planning phase. Setup instructions will be added once the extension scaffold is in place.)*

## Pull Request Process

1. **Fork & branch.** Create a feature branch from `main` (e.g., `feature/dom-sanitizer`).
2. **DCO required.** All commits must be signed off under the [Developer Certificate of Origin](https://developercertificate.org/):
   ```
   Signed-off-by: Your Name <your.email@example.com>
   ```
   Use `git commit -s` to add the sign-off automatically.
3. **Test your changes.** Ensure nothing breaks the safety baseline.
4. **Update documentation.** Any change to security behavior, data flow, or risk controls must update the relevant docs and `CHANGELOG.md`.
5. **Open a PR.** Describe the change, its motivation, and any security implications.

## Review Requirements

| Change type | Review required |
|---|---|
| Bug fix, docs, refactor | One maintainer approval |
| New feature | One maintainer approval + public discussion |
| **Security baseline / data flow / risk control** | **Two maintainer approvals (dual review)** |
| Governance charter amendment | Public proposal + community review period |

Security-sensitive changes must not be merged until dual review is complete. This is a non-negotiable rule per [GOVERNANCE.md](GOVERNANCE.md).

## Reporting Issues

- **Bugs / feature requests**: Use the GitHub Issue templates.
- **Security vulnerabilities**: Use the Security Report issue template. Do not disclose vulnerabilities publicly until a fix is available.

## Licensing

By contributing, you agree that your contributions are licensed under the GNU GPLv3 with the Public Paradigm Supervision Additional Terms. See [LICENSE](LICENSE).
