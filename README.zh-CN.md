# FocusView

[English](README.md) | **简体中文**

> 公共生成式Web交互范式 — 自然语言驱动的浏览器本地DOM重构。

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![Public Paradigm](https://img.shields.io/badge/Paradigm-Public%20%26%20Supervised-green.svg)](GOVERNANCE.zh-CN.md)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

## FocusView 是什么？

FocusView 是一个浏览器扩展（Manifest V3），让用户用自然语言重塑任意网页。用户无需接受网站的固定布局，只需描述意图——"隐藏广告、放大字体、去掉侧边栏、切换暗色模式"——生成式AI模型即生成 CSS/JS，由扩展在本地实时注入。

**所有修改均在浏览器本地发生，远端网站不会被任何改动。**

## 为什么是"公共范式"？

重塑你所看到的网页的能力应当属于每个人——不应被私有产品锁定。本项目将交互范式本身定义为公共资源，由社区监管而非私人控制。

完整治理章程见 [GOVERNANCE.zh-CN.md](GOVERNANCE.zh-CN.md)。

## 安全第一

FocusView 强制执行不可协商的安全基线：

- **默认模式：仅 CSS。** AI 生成的 JavaScript 默认被丢弃。
- **JS 执行需主动开启。** 用户必须手动启用，并看到明确的风险警告。
- **DOM 脱敏。** 密码字段和敏感表单数据在发送给 AI 前被剥离。
- **密钥仅存本地。** API 密钥永不离开浏览器。
- **禁止远程代码。** 严格 CSP；所有可执行代码随扩展包发布。

详见 [SECURITY.zh-CN.md](SECURITY.zh-CN.md)。

## 文档索引

| 文档 | English | 简体中文 |
|---|---|---|
| 项目说明 | [README.md](README.md) | [README.zh-CN.md](README.zh-CN.md) |
| 治理章程 | [GOVERNANCE.md](GOVERNANCE.md) | [GOVERNANCE.zh-CN.md](GOVERNANCE.zh-CN.md) |
| 安全策略 | [SECURITY.md](SECURITY.md) | [SECURITY.zh-CN.md](SECURITY.zh-CN.md) |
| 贡献指南 | [CONTRIBUTING.md](CONTRIBUTING.md) | — |
| 变更日志 | [CHANGELOG.md](CHANGELOG.md) | — |

## 开源协议

FocusView 基于 **GNU 通用公共许可证 v3.0** 并附加 **公共范式监管附加条款** 开源。

- GPLv3 确保所有衍生分发版本保持开源。
- 附加条款（GPLv3 第 7 节）确立公共安全基线，禁止将范式私有化。

完整文本见 [LICENSE](LICENSE)。

版权所有 (C) 2026 ccccwwwxx / Shone Cui

## 项目状态

本仓库目前包含项目基础文件：开源协议、治理章程、安全策略和社区健康文件。实现代码正在规划中。

## 贡献

所有贡献均需遵循 DCO（开发者来源证书）。安全相关变更须按治理章程进行双重评审。详见 [CONTRIBUTING.md](CONTRIBUTING.md)。
