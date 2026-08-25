# Security Policy & Public Baseline
## 安全策略与公众监管基线

### Project Security Position / 项目安全定位

This project realizes generative AI-driven local webpage reconstruction.
To protect public user rights and paradigm credibility,
all security mechanisms are open, auditable, and community-supervised.

本项目实现生成式AI驱动的本地网页重构。
为保护公众用户权益和范式公信力，
所有安全机制开放、可审计、接受社区监管。

---

### Core Security Baseline / 核心安全基线（硬编码 & 公开锁定）

#### 1. Capability Stratification / 能力分层

- **Safe Default Mode / 安全默认模式**: Only parse and execute AI-generated CSS; discard all JavaScript code.
  仅解析并执行AI生成的CSS，丢弃所有JS代码。
- **Advanced Dangerous Mode / 高级危险模式**: Manual user activation + prominent red risk warning;
  strictly user-discretion liability.
  用户手动激活 + 显著红色风险警告，责任由用户自行承担。

#### 2. Data Desensitization Mechanism / 数据脱敏机制

Automatic filtering of all sensitive DOM nodes before uploading to AI:
- Password input fields (`input[type="password"]`)
- Hidden form values
- User private form data (credit card, ID numbers, etc.)

上传AI前自动过滤所有敏感DOM节点：
- 密码输入框
- 隐藏表单值
- 用户隐私表单数据（信用卡、身份证号等）

#### 3. Local-only Privacy Protection / 本地隐私保护

- User API Key stored only in browser local storage (`chrome.storage.local`).
  用户API Key仅存储在浏览器本地存储中。
- No backend data collection, no stealth upload behavior.
  无后端数据收集，无偷传行为。
- Local operation only; no remote data reporting.
  纯本地运行，无远程数据上报。

#### 4. CSP Strict Restriction / CSP严格限制

- Manifest V3 standard strict Content Security Policy.
  遵循Manifest V3标准严格内容安全策略。
- Prohibit remote dynamic script injection.
  禁止远程动态脚本注入。
- All executable code must be packaged within the extension; no remote code loading.
  所有可执行代码必须打包在扩展内，禁止远程加载代码。
- Eliminate backdoor remote control risks.
  消除后门远程控制风险。

#### 5. Auditability / 可审计性

- Local behavior log reserved for user self-audit (DOM uploads, API calls, code execution).
  保留本地行为日志供用户自审（DOM上传、API调用、代码执行记录）。
- All core logic is open source for full public audit.
  所有核心逻辑开源，接受全面公众审计。
- Release packages provide source hash for verification.
  发布版本提供源码哈希供校验。

---

### Vulnerability Disclosure / 漏洞披露

- Public GitHub Issues channel for security vulnerability reporting.
  通过GitHub Issues公开渠道报告安全漏洞。
- All security fixes are publicly disclosed and recorded in CHANGELOG.
  所有安全修复公开披露并记录在CHANGELOG中。
- Reporters will be acknowledged in security advisories.
  报告者将在安全公告中署名致谢。

---

### Risk Disclaimer / 风险免责声明

This paradigm is a public open technical exploration.
The advanced manual-enabled AI dynamic code execution mode carries inherent risks.
All usage behaviors are the independent choice of the user.
The authors and community contributors do not assume corresponding liability.
See the GNU General Public License version 3, Sections 15 and 16 for the full disclaimer.

本范式是公共开放的技术探索。
高级手动开启的AI动态代码执行模式具有固有风险。
所有使用行为均为用户的自主选择。
作者和社区贡献者不承担相应责任。
完整免责声明见GNU通用公共许可证第3版第15、16条。
