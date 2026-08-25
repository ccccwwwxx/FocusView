# FocusView

**English** | [简体中文](README.zh-CN.md)

> A public generative web interaction paradigm — natural language-driven local browser DOM reconstruction.

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![Public Paradigm](https://img.shields.io/badge/Paradigm-Public%20%26%20Supervised-green.svg)](GOVERNANCE.md)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

## What is FocusView?

FocusView is a browser extension (Manifest V3) that lets users reshape any webpage using natural language. Instead of accepting a website's fixed layout, users describe their intent — "hide ads, enlarge the font, remove the sidebar, switch to dark mode" — and a generative AI model produces the CSS/JS that the extension injects locally, in real time.

**All modifications happen locally in the browser. The remote website is never altered.**

## Why "Public Paradigm"?

The ability to reshape the web you see should belong to everyone — not locked behind a proprietary product. This project defines the interaction paradigm itself as a public resource, governed by community supervision rather than private control.

See [GOVERNANCE.md](GOVERNANCE.md) for the full governance charter.

## Safety First

FocusView enforces a non-negotiable safety baseline:

- **Default mode: CSS-only.** AI-generated JavaScript is discarded by default.
- **JS execution is opt-in.** Users must manually enable it with explicit risk warnings.
- **DOM desensitization.** Password fields and sensitive form data are stripped before any AI request.
- **Local-only keys.** API keys never leave the browser.
- **No remote code.** Strict CSP; all executable code ships in the extension package.

See [SECURITY.md](SECURITY.md) for details.

## Documentation

| Document | English | 简体中文 |
|---|---|---|
| Project overview | [README.md](README.md) | [README.zh-CN.md](README.zh-CN.md) |
| Governance charter | [GOVERNANCE.md](GOVERNANCE.md) | [GOVERNANCE.zh-CN.md](GOVERNANCE.zh-CN.md) |
| Security policy | [SECURITY.md](SECURITY.md) | [SECURITY.zh-CN.md](SECURITY.zh-CN.md) |
| Contributing guide | [CONTRIBUTING.md](CONTRIBUTING.md) | — |
| Changelog | [CHANGELOG.md](CHANGELOG.md) | — |

## License

FocusView is licensed under the **GNU General Public License v3.0** with **Public Paradigm Supervision Additional Terms**.

- The GPLv3 ensures all derivative distributions remain open source.
- The additional terms (under GPLv3 Section 7) enshrine the public safety baseline and prohibit privatization of the paradigm.

See [LICENSE](LICENSE) for the full text.

Copyright (C) 2026 ccccwwwxx / Shone Cui

## Project Status

This repository currently holds the project's foundational documents: license, governance charter, security policy, and community health files. Implementation is in the planning phase.

## Contributing

All contributions are welcome under the DCO (Developer Certificate of Origin). Security-related changes require dual review per the governance charter. See [CONTRIBUTING.md](CONTRIBUTING.md) for details.
