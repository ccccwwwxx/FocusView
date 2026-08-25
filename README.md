# FocusView

> A public generative web interaction paradigm — natural language-driven local browser DOM reconstruction.
> 公共生成式Web交互范式 — 自然语言驱动的浏览器本地DOM重构。

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![Public Paradigm](https://img.shields.io/badge/Paradigm-Public%20%26%20Supervised-green.svg)](GOVERNANCE.md)

## What is FocusView? / FocusView是什么？

FocusView is a browser extension (Manifest V3) that lets users reshape any webpage using natural language. Instead of accepting a website's fixed layout, users describe their intent — "hide ads, enlarge the font, remove the sidebar, switch to dark mode" — and a generative AI model produces the CSS/JS that the extension injects locally, in real time.

FocusView是一个浏览器扩展（Manifest V3），让用户用自然语言重塑任意网页。用户无需接受网站的固定布局，只需描述意图——"隐藏广告、放大字体、去掉侧边栏、切换暗色模式"——生成式AI模型即生成CSS/JS，由扩展在本地实时注入。

**All modifications happen locally in the browser. The remote website is never altered.**
**所有修改均在浏览器本地发生，远端网站不会被任何改动。**

## Why "Public Paradigm"? / 为什么是"公共范式"？

The ability to reshape the web you see should belong to everyone — not locked behind a proprietary product. This project defines the interaction paradigm itself as a public resource, governed by community supervision rather than private control.

重塑你所看到的网页的能力应当属于每个人——不应被私有产品锁定。本项目将交互范式本身定义为公共资源，由社区监管而非私人控制。

See [GOVERNANCE.md](GOVERNANCE.md) for the full governance charter.

## Safety First / 安全第一

FocusView enforces a non-negotiable safety baseline:

- **Default mode: CSS-only.** AI-generated JavaScript is discarded by default.
- **JS execution is opt-in.** Users must manually enable it with explicit risk warnings.
- **DOM desensitization.** Password fields and sensitive form data are stripped before any AI request.
- **Local-only keys.** API keys never leave the browser.
- **No remote code.** Strict CSP; all executable code ships in the extension package.

See [SECURITY.md](SECURITY.md) for details.

## License / 开源协议

FocusView is licensed under the **GNU General Public License v3.0** with **Public Paradigm Supervision Additional Terms**.

- The GPLv3 ensures all derivative distributions remain open source.
- The additional terms (under GPLv3 Section 7) enshrine the public safety baseline and prohibit privatization of the paradigm.

See [LICENSE](LICENSE) for the full text.

Copyright (C) 2026 ccccwwwxx / Shone Cui

## Project Status / 项目状态

This repository currently holds the project's foundational documents: license, governance charter, and security policy. Implementation is in the planning phase.

本仓库目前包含项目基础文件：开源协议、治理章程和安全策略。实现代码正在规划中。

## Contributing / 贡献

All contributions are welcome under the DCO (Developer Certificate of Origin). Security-related changes require dual review per the governance charter.
