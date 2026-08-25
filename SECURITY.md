# Security Policy & Public Baseline

**English** | [简体中文](SECURITY.zh-CN.md)

## Project Security Position

This project realizes generative AI-driven local webpage reconstruction. To protect public user rights and paradigm credibility, all security mechanisms are open, auditable, and community-supervised.

## Core Security Baseline (Hard-coded & Public Locked)

### 1. Capability Stratification

- **Safe Default Mode**: Only parse and execute AI-generated CSS; discard all JavaScript code.
- **Advanced Dangerous Mode**: Manual user activation + prominent red risk warning; strictly user-discretion liability.

### 2. Data Desensitization Mechanism

Automatic filtering of all sensitive DOM nodes before uploading to AI:

- Password input fields (`input[type="password"]`)
- Hidden form values
- User private form data (credit card, ID numbers, etc.)

### 3. Local-only Privacy Protection

- User API Key stored only in browser local storage (`chrome.storage.local`).
- No backend data collection, no stealth upload behavior.
- Local operation only; no remote data reporting.

### 4. CSP Strict Restriction

- Manifest V3 standard strict Content Security Policy.
- Prohibit remote dynamic script injection.
- All executable code must be packaged within the extension; no remote code loading.
- Eliminate backdoor remote control risks.

### 5. Auditability

- Local behavior log reserved for user self-audit (DOM uploads, API calls, code execution).
- All core logic is open source for full public audit.
- Release packages provide source hash for verification.

## Vulnerability Disclosure

- Public GitHub Issues channel for security vulnerability reporting.
- All security fixes are publicly disclosed and recorded in [CHANGELOG.md](CHANGELOG.md).
- Reporters will be acknowledged in security advisories.

## Risk Disclaimer

This paradigm is a public open technical exploration. The advanced manual-enabled AI dynamic code execution mode carries inherent risks. All usage behaviors are the independent choice of the user. The authors and community contributors do not assume corresponding liability. See the GNU General Public License version 3, Sections 15 and 16 for the full disclaimer.
