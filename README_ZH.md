# 🦞 Awesome OpenClaw Family (OpenClaw 生态精选)

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
[![Contributions Welcome](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](#-contributing)
[![License: CC0](https://img.shields.io/badge/License-CC0--1.0-lightgrey.svg)](LICENSE)
[![Stars](https://img.shields.io/github/stars/YOUR_GITHUB_USERNAME/Awesome-OpenClaw-Family?style=social)](https://github.com/YOUR_GITHUB_USERNAME/Awesome-OpenClaw-Family/stargazers)

*一份经过严格筛选的 OpenClaw 生态系统地图：涵盖核心运行时、通道、技能注册表、工作流 Shell、安全加固、部署方案以及真实世界的使用案例。*

> 如果这个仓库帮助你构建了更好的本地优先助手，请给它一个 Star。

**维护者:** `@wu-yc` · **欢迎 PR** · **快照日期:** **2026-02-18** (在此日期之后指标可能会略有偏差)

---

## 🧭 概览 (Overview)

OpenClaw 是一个运行在你自有设备上的本地优先个人 AI 助手，旨在通过你已经使用的消息通道工作，并通过技能市场 + 可组合的工作流 Shell 进行扩展。这份列表专注于 **规范的** OpenClaw 家族项目（官方仓库优先）、**经过验证的** 生态系统组件（技能、加固、部署）以及对生产级本地代理至关重要的 **高信号** 衍生品（分支/重实现）。

---

## 🗞️ 新闻 (News)

- (2026-02-18) **本仓库**: 重写为符合 “Awesome-Agentic-Labs-grade” 规范（分类体系 + 统一条目 + 工作流阶段 + 领域应用）。
- (2026-02-18) **OpenClaw × VirusTotal**: 宣布官方合作伙伴关系，用于技能和构件扫描。
- (2026-02-17) **OpenClaw**: 稳定发布线持续更新（见 GitHub releases）。
- (2026-02-04) **技能市场风险**: 公开报道强调了恶意技能和供应链担忧。
- (2026-01-29) **重命名**: OpenClaw 推出（前身为 Moltbot / Clawdbot）。

---

## 🧾 规范 (Conventions)

### 分类体系 (Taxonomy)

每个条目遵循：

`(YYYY-MM-DD) **名称** [📝 论文] [💻 仓库] [🌐 网站] [📄 文档] *≤25字描述。* (类型: ..., 成熟度: ..., 集成方式: ..., 许可证: ..., Stars: ...)`

**类型 (Type)**
- **Assistant**: 主要的本地代理运行时。
- **Gateway/Control Plane**: 编排、配置、会话控制。
- **Channel**: WhatsApp/Telegram/Slack 等连接器。
- **Skill Registry**: 发现、索引、分发。
- **Skill**: 可调用的能力包（通常通过 ClawHub）。
- **Workflow Engine**: 类型化管道 / 审批门控 / 确定性自动化。
- **Security**: 威胁模型、扫描器、加固套件。
- **Packaging/Deploy**: 安装程序、Nix/Homebrew、Ansible、基础设施模块。
- **Derivative**: Claw 家族中的分支、重实现、替代品。

**成熟度 (Maturity)**
- **Production**: 广泛使用，接口稳定，积极维护。
- **Active**: 维护中 + 可用，可能会变动。
- **Beta**: 功能正常但在演进中。
- **Experimental**: 早期阶段，接口不稳定。
- **Archived**: 已冻结，具有历史价值。

**集成方式 (Integration)**
- **Local-only**: 默认无出站网络访问。
- **CLI Wrapper**: 包装本地 CLI 工具 (gh/op/etc)。
- **Gateway Skill**: 安装到 OpenClaw 代理环境中。
- **Service**: 涉及外部托管 API/服务。
- **Registry**: 目录 / 市场 / 索引。

### 链接 (Links)

- 优先使用 **官方** GitHub 仓库和官方文档/网站。
- 如果不存在规范仓库，提供 **GitHub 搜索** 链接。
- 对于技能，优先使用 **ClawHub 技能页面**；如果上游代码模棱两可，请明确标记。

---

## 📌 目录 (Content)

- [1. OpenClaw 核心 (官方)](#1-openclaw-核心-官方)
- [2. 分支与重实现](#2-分支与重实现)
- [3. 相似项目与替代品](#3-相似项目与替代品)
- [4. 技能与扩展](#4-技能与扩展)
- [5. 真实应用案例](#5-真实应用案例)
- [6. 安全](#6-安全)
- [7. 部署](#7-部署)
- [8. 社区](#8-社区)
- [工作流阶段](#-工作流阶段)
- [领域应用](#-领域应用)
- [9. 相关 Awesome 列表](#9-相关-awesome-列表)
- [10. 贡献指南](#10-贡献指南)
- [11. 关键引用](#11-关键引用)
- [12. Star 历史](#12-star-历史)

---

## 1. OpenClaw 核心 (官方)

### 核心运行时与文档

- (2026-02-18) **OpenClaw** [💻 仓库](https://github.com/openclaw/openclaw) [🌐 网站](https://openclaw.ai) [📄 文档](https://docs.openclaw.ai) *具有多通道聊天、技能和工作流的本地优先个人 AI 助手。* (类型: Assistant, 成熟度: Production, 集成方式: Gateway, 许可证: MIT, Stars: ~209k)

- (2026-02-18) **OpenClaw 安装指南** [📄 文档](https://docs.openclaw.ai/install) *安装程序 + 特定平台安装路径 (macOS/Linux/Windows via WSL2)。* (类型: Packaging/Deploy, 成熟度: Production, 集成方式: Docs, 许可证: —, Stars: —)

- (2026-02-18) **openclaw.ai (网站仓库)** [💻 仓库](https://github.com/openclaw/openclaw.ai) [🌐 网站](https://openclaw.ai) *官方网站和分发入口的源码。* (类型: Gateway/Control Plane, 成熟度: Active, 集成方式: Site, 许可证: —, Stars: ~171)

### 技能注册表与市场

- (2026-02-18) **ClawHub** [💻 仓库](https://github.com/openclaw/clawhub) [🌐 网站](https://clawhub.ai) *OpenClaw 的技能注册表，具有快速发现和索引功能。* (类型: Skill Registry, 成熟度: Production, 集成方式: Registry, 许可证: MIT, Stars: ~2.3k)

- (2026-02-18) **openclaw/skills (归档)** [💻 仓库](https://github.com/openclaw/skills) *发布到 clawdhub.com 的技能的历史版本归档。* (类型: Skill Registry, 成熟度: Archived, 集成方式: Registry, 许可证: MIT, Stars: ~1.1k)

### 工作流 Shell

- (2026-02-18) **Lobster** [💻 仓库](https://github.com/openclaw/lobster) *类型化的本地优先工作流 Shell：用于代理自动化的管道、作业和审批门控。* (类型: Workflow Engine, 成熟度: Active, 集成方式: Local-only, 许可证: MIT, Stars: ~506)

### 安全典范

- (2026-02-18) **OpenClaw Trust** [💻 仓库](https://github.com/openclaw/trust) [🌐 网站](https://trust.openclaw.ai) *机器可检查的威胁模型 + 映射到 MITRE ATLAS 的缓解措施。* (类型: Security, 成熟度: Active, 集成方式: Docs, 许可证: —, Stars: ~116)

### 打包与运维 (官方)

- (2026-02-18) **nix-openclaw** [💻 仓库](https://github.com/openclaw/nix-openclaw) *OpenClaw 的 Nix 打包。* (类型: Packaging/Deploy, 成熟度: Active, 集成方式: Local-only, 许可证: —, Stars: ~399)

- (2026-02-18) **openclaw-ansible** [💻 仓库](https://github.com/openclaw/openclaw-ansible) *加固的安装自动化（Tailscale VPN, UFW 防火墙, Docker 隔离）。* (类型: Packaging/Deploy, 成熟度: Active, 集成方式: Host/Infra, 许可证: MIT, Stars: ~346)

- (2026-02-18) **homebrew-tap** [💻 仓库](https://github.com/openclaw/homebrew-tap) *官方 Homebrew tap。* (类型: Packaging/Deploy, 成熟度: Active, 集成方式: Local-only, 许可证: —, Stars: ~27)

- (2026-02-18) **clawdinators** [💻 仓库](https://github.com/openclaw/clawdinators) *用于 “CLAWTINATOR” 主机的声明式基础设施 + NixOS 模块。* (类型: Packaging/Deploy, 成熟度: Active, 集成方式: Host/Infra, 许可证: MIT, Stars: ~109)

- (2026-02-18) **clawgo** [💻 仓库](https://github.com/openclaw/clawgo) *Clawd 节点的 Go 实现。* (类型: Derivative, 成熟度: Experimental, 集成方式: Local-only, 许可证: MIT, Stars: ~33)

### 官方副项目

- (2026-02-18) **Casa** [💻 仓库](https://github.com/openclaw/casa) *macOS 上用于自动化/代理的本地 HomeKit 桥接 (REST API + CLI)。* (类型: Channel, 成熟度: Experimental, 集成方式: Local-only, 许可证: —, Stars: ~24)

- (2026-02-18) **butter.bot** [💻 仓库](https://github.com/openclaw/butter.bot) [🌐 网站](https://butter.bot) *微型官方副项目网站仓库 (HTML)。* (类型: Community, 成熟度: Experimental, 集成方式: Site, 许可证: MIT, Stars: ~7)

- (2026-02-18) **voice-community** [💻 仓库](https://github.com/openclaw/voice-community) *语音相关实验的社区草稿空间。* (类型: Community, 成熟度: Experimental, 集成方式: Local-only, 许可证: —, Stars: ~4)

- (2026-02-18) **barnacle** [💻 仓库](https://github.com/openclaw/barnacle) *小型实用工具机器人 (“sticks around”)。* (类型: Community, 成熟度: Experimental, 集成方式: Bot, 许可证: —, Stars: ~14)

---

## 2. 分支与重实现

> 仅包含真实的、可发现的、高信号的衍生品。官方 OpenClaw 仍是规范。

- (2026-02-18) **NanoClaw** [💻 仓库](https://github.com/qwibitai/nanoclaw) *专注于安全和多通道使用的容器优先轻量级替代品。* (类型: Derivative, 成熟度: Active, 集成方式: Container, 许可证: MIT, Stars: ~8.9k)

- (2026-02-18) **nanobot** [💻 仓库](https://github.com/HKUDS/nanobot) *受 OpenClaw 启发的超轻量级助手（小型，核心可审计）。* (类型: Derivative, 成熟度: Active, 集成方式: Local-only, 许可证: MIT, Stars: ~20.8k)

- (2026-02-18) **PicoClaw** [💻 仓库](https://github.com/sipeed/picoclaw) [🌐 网站](https://picoclaw.ai) *基于 Go 的超轻助手，针对低资源硬件。* (类型: Derivative, 成熟度: Active, 集成方式: Local-only, 许可证: MIT, Stars: ~8.4k)

- (2026-02-18) **ZeroClaw** [💻 仓库](https://github.com/zeroclaw-labs/zeroclaw) [🌐 网站](https://zeroclaw.org) *基于 Rust 的“代理运行时内核”风格的 Claw 家族重构。* (类型: Derivative, 成熟度: Active, 集成方式: Local-only, 许可证: —, Stars: ~13.6k)

- (2026-02-18) **femtoclaw** [💻 仓库](https://github.com/mcotdev/femtoclaw) *极小的基于 Rust 的 OpenClaw 变体（最小占用）。* (类型: Derivative, 成熟度: Experimental, 集成方式: Local-only, 许可证: MIT, Stars: ~4)

- (2026-02-18) **IronClaw (NEAR AI)** [💻 仓库](https://github.com/nearai/ironclaw) *强调沙盒和能力风格控制的 Rust 重实现。* (类型: Derivative, 成熟度: Active, 集成方式: Local-only, 许可证: —, Stars: —)

---

## 3. 相似项目与替代品

> 通常围绕 OpenClaw 部署使用的相邻构建块和生态系统桥梁。

- (2026-02-18) **skills.sh (生态系统)** [🌐 网站](https://skills.sh) *ClawHub 工具引用的独立技能注册表生态系统。* (类型: Skill Registry, 成熟度: Active, 集成方式: Registry, 许可证: —, Stars: —)

- (2026-02-18) **MITRE ATLAS** [🌐 网站](https://atlas.mitre.org) *AI 赋能系统的对抗性威胁知识库；用于 OpenClaw Trust 映射。* (类型: Security, 成熟度: Production, 集成方式: Reference, 许可证: —, Stars: —)

---

## 4. 技能与扩展

> **高信号** ClawHub 技能的精选快照（官方 + 流行 + 安全相关）。
>
> **关于指标的说明：** 对于技能，“Stars” 和 “Downloads” 指的是技能页面上可见的 **ClawHub** 计数器。

### 4.1 核心 / 维护者技能 (ClawHub)

- (2026-02-18) **Notion** [🧩 技能](https://clawhub.ai/steipete/notion) *用于页面/数据库/块的 Notion API 助手。* (类型: Skill, 成熟度: Active, 集成方式: Gateway Skill, 许可证: N/A, Stars: ⭐28, Downloads: ~9.5k)

- (2026-02-18) **Weather** [🧩 技能](https://clawhub.ai/steipete/weather) *无需 API 密钥的天气 + 预报。* (类型: Skill, 成熟度: Active, 集成方式: CLI Wrapper, 许可证: N/A, Stars: ⭐25, Downloads: ~15.6k)

- (2026-02-18) **1Password** [🧩 技能](https://clawhub.ai/steipete/1password) *1Password CLI (`op`) 使用，用于安全秘密注入。* (类型: Skill, 成熟度: Active, 集成方式: CLI Wrapper, 许可证: N/A, Stars: ⭐10, Downloads: ~4k)

- (2026-02-18) **Spotify Player** [🧩 技能](https://clawhub.ai/steipete/spotify-player) *通过 CLI 进行终端 Spotify 播放/搜索。* (类型: Skill, 成熟度: Active, 集成方式: CLI Wrapper, 许可证: N/A, Stars: ⭐6, Downloads: ~4.5k)

- (2026-02-18) **GitHub (gh CLI)** [🧩 技能](https://clawhub.ai/steipete/github) *使用 `gh` 处理 PR、issue 和 CI 运行。* (类型: Skill, 成熟度: Active, 集成方式: CLI Wrapper, 许可证: N/A, Stars: —)

- (2026-02-18) **Clawdhub CLI** [🧩 技能](https://clawhub.ai/steipete/clawdhub) *通过 ClawdHub 搜索/安装/更新/发布技能。* (类型: Skill, 成熟度: Active, 集成方式: CLI Wrapper, 许可证: N/A, Stars: —)

- (2026-02-18) **Apple Reminders** [🧩 技能](https://clawhub.ai/steipete/apple-reminders) *通过 CLI 管理 macOS 上的 Apple 提醒事项。* (类型: Skill, 成熟度: Active, 集成方式: CLI Wrapper, 许可证: N/A, Stars: —)

- (2026-02-18) **Peekaboo** [🧩 技能](https://clawhub.ai/steipete/peekaboo) *使用本地 CLI 捕获/自动化 macOS UI。* (类型: Skill, 成熟度: Active, 集成方式: CLI Wrapper, 许可证: N/A, Stars: —)

- (2026-02-18) **OpenAI Image Gen** [🧩 技能](https://clawhub.ai/steipete/openai-image-gen) *通过 OpenAI Images API 批量生成图像并带有本地图库。* (类型: Skill, 成熟度: Active, 集成方式: Service, 许可证: N/A, Stars: —)

- (2026-02-18) **Blogwatcher** [🧩 技能](https://clawhub.ai/steipete/blogwatcher) *通过 CLI 监控 RSS/Atom 源更新。* (类型: Skill, 成熟度: Active, 集成方式: CLI Wrapper, 许可证: N/A, Stars: —)

- (2026-02-18) **Gog (Google Workspace CLI)** [🧩 技能](https://clawhub.ai/steipete/gog) *Google Workspace CLI 工作流 (Gmail/Calendar/Drive/etc)。* (类型: Skill, 成熟度: Active, 集成方式: CLI Wrapper, 许可证: N/A, Stars: —)

- (2026-02-18) **Things (macOS)** [🧩 技能](https://www.clawhub.ai/steipete/things-mac) *通过 CLI + 本地数据库管理 Things 3 任务/项目。* (类型: Skill, 成熟度: Active, 集成方式: CLI Wrapper, 许可证: N/A, Stars: —)

### 4.2 流行实用技能 (ClawHub)

- (2026-02-18) **Ontology** [🧩 技能](https://clawhub.ai/oswalpalash/ontology) *用于代理知识的结构化本体创建 + 转换。* (类型: Skill, 成熟度: Active, 集成方式: Gateway Skill, 许可证: N/A, Stars: ⭐19, Downloads: ~17.3k)

- (2026-02-18) **Google Slides** [🧩 技能](https://clawhub.ai/byungkyu/google-slides) *通过托管 OAuth 网关创建和编辑 Google 幻灯片。* (类型: Skill, 成熟度: Active, 集成方式: Service, 许可证: N/A, Stars: ⭐10, Downloads: ~7.2k)

- (2026-02-18) **Apple Calendar** [🧩 技能](https://clawhub.ai/tyler6204/apple-calendar) *通过脚本对 macOS 日历事件进行 CRUD 操作。* (类型: Skill, 成熟度: Active, 集成方式: CLI Wrapper, 许可证: N/A, Stars: ⭐7, Downloads: ~1.5k)

- (2026-02-18) **Apple Calendar CLI** [🧩 技能](https://clawhub.ai/joargp/accli) *替代的 Apple Calendar CLI 指令集。* (类型: Skill, 成熟度: Active, 集成方式: CLI Wrapper, 许可证: N/A, Stars: —)

- (2026-02-18) **Caldav Calendar** [🧩 技能](https://clawhub.ai/Asleep123/caldav-calendar) *通过 vdirsyncer + khal 进行 CalDAV 同步/查询。* (类型: Skill, 成熟度: Active, 集成方式: CLI Wrapper, 许可证: N/A, Stars: —)

- (2026-02-18) **Google Calendar (gcalcli)** [🧩 技能](https://clawhub.ai/lstpsche/gcalcli-calendar) *通过 gcalcli 进行低调用量的 Google Calendar 工作流。* (类型: Skill, 成熟度: Active, 集成方式: CLI Wrapper, 许可证: N/A, Stars: —)

- (2026-02-18) **Google Calendar (API)** [🧩 技能](https://clawhub.ai/AdrianMiller99/google-calendar) *通过 API 进行编程化 Google Calendar 操作。* (类型: Skill, 成熟度: Active, 集成方式: Service, 许可证: N/A, Stars: —)

- (2026-02-18) **Calendar (generic)** [🧩 技能](https://clawhub.ai/0xterrybit/calendar) *日历管理和调度。* (类型: Skill, 成熟度: Active, 集成方式: Service, 许可证: N/A, Stars: —)

- (2026-02-18) **Gmail Agent** [🧩 技能](https://clawhub.ai/r39132/gmail-agent) *总结未读 Gmail；审计标签；清除垃圾邮件/回收站。* (类型: Skill, 成熟度: Active, 集成方式: Service, 许可证: N/A, Stars: —)

- (2026-02-18) **Clawemail (Google Workspace service)** [🧩 技能](https://clawhub.ai/cto1/clawemail) *通过服务进行 Workspace 操作 (Gmail/Drive/Docs/Sheets/Calendar)。* (类型: Skill, 成熟度: Active, 集成方式: Service, 许可证: N/A, Stars: —)

- (2026-02-18) **Himalaya** [🧩 技能](https://clawhub.ai/skills/himalaya) *通过 IMAP/SMTP 进行终端邮件操作 (himalaya CLI)。* (类型: Skill, 成熟度: Active, 集成方式: CLI Wrapper, 许可证: N/A, Stars: —)

- (2026-02-18) **React Email Skills** [🧩 技能](https://clawhub.ai/christina-de-martinez/react-email-skills) *使用 React Email 生成响应式 HTML 邮件。* (类型: Skill, 成熟度: Active, 集成方式: Gateway Skill, 许可证: N/A, Stars: —)

- (2026-02-18) **Clippy (Microsoft 365 CLI)** [🧩 技能](https://clawhub.ai/foeken/clippy) *通过 CLI 管理 Outlook/M365 邮件 + 日历。* (类型: Skill, 成熟度: Active, 集成方式: CLI Wrapper, 许可证: N/A, Stars: —)

### 4.3 安全、审查与治理 (ClawHub)

- (2026-02-18) **Skill Vetter** [🧩 技能](https://clawhub.ai/steipete/skill-vetter) *针对可疑技能模式的自动化审查管道。* (类型: Skill, 成熟度: Active, 集成方式: Gateway Skill, 许可证: N/A, Stars: ⭐7, Downloads: ~2.6k)

- (2026-02-18) **Skill Scanner** [🧩 技能](https://clawhub.ai/bvinci1-design/skill-scanner) *带有 UI 的本地恶意模式静态扫描器。* (类型: Skill, 成熟度: Active, 集成方式: Local-only, 许可证: N/A, Stars: ⭐5, Downloads: ~1.9k)

- (2026-02-18) **AI Skill Scanner** [🧩 技能](https://clawhub.ai/HugoSbl/ai-skill-scanner) *扫描技能中的漏洞和可疑模式。* (类型: Skill, 成熟度: Active, 集成方式: Gateway Skill, 许可证: N/A, Stars: —)

- (2026-02-18) **Skill Defender** [🧩 技能](https://clawhub.ai/itsclawdbro/skill-defender) *扫描已安装技能中的提示注入、数据渗漏、后门。* (类型: Skill, 成熟度: Active, 集成方式: Gateway Skill, 许可证: N/A, Stars: —)

- (2026-02-18) **Sammā Suit** [🧩 技能](https://clawhub.ai/OneZeroEight-ai/samma-suit) *治理层：预算、权限、审计日志、终止开关、审查。* (类型: Skill, 成熟度: Active, 集成方式: Gateway Skill, 许可证: N/A, Stars: —)

### 4.4 研究、Web 与浏览 (ClawHub)

- (2026-02-18) **Google Search (grounding)** [🧩 技能](https://clawhub.ai/Shaharsha/google-search-grounding) *通过 Gemini Search Grounding + 回退 API 进行网络搜索。* (类型: Skill, 成熟度: Active, 集成方式: Service, 许可证: N/A, Stars: —)

- (2026-02-18) **MCP Skill** [🧩 技能](https://clawhub.ai/simlocker/mcp-skill) *包装 MCP 服务器用于网络搜索/深度研究/爬取/公司研究。* (类型: Skill, 成熟度: Active, 集成方式: Service, 许可证: N/A, Stars: —)

- (2026-02-18) **Fastest Browser Use** [🧩 技能](https://clawhub.ai/rknoche6/fast-browser-use) *用于抓取和 DOM 提取的高性能浏览器自动化。* (类型: Skill, 成熟度: Active, 集成方式: Gateway Skill, 许可证: N/A, Stars: —)

- (2026-02-18) **Agent Browser (v3)** [🧩 技能](https://clawhub.ai/tekkenKK/agent-browser-3) *用于 Web 测试/表单/截图的浏览器自动化指令。* (类型: Skill, 成熟度: Active, 集成方式: Gateway Skill, 许可证: N/A, Stars: —)

- (2026-02-18) **Agent Browser (Clawdbot)** [🧩 技能](https://clawhub.ai/MaTriXy/agent-browser-clawdbot) *agent-browser CLI 的仅指令包装器。* (类型: Skill, 成熟度: Active, 集成方式: CLI Wrapper, 许可证: N/A, Stars: —)

- (2026-02-18) **DeepWiki** [🧩 技能](https://clawhub.ai/arun-8687/deepwiki) *查询 DeepWiki MCP 服务器以获取 GitHub 仓库文档和问答。* (类型: Skill, 成熟度: Active, 集成方式: Service, 许可证: N/A, Stars: —)

- (2026-02-18) **Skills.sh Search** [🧩 技能](https://clawhub.ai/TheSethRose/skills-search) *从 CLI 搜索 skills.sh 注册表。* (类型: Skill, 成熟度: Active, 集成方式: CLI Wrapper, 许可证: N/A, Stars: ⭐3, Downloads: ~2k)

### 4.5 记忆、角色与 Agent 运维 (ClawHub)

- (2026-02-18) **Memory Tools** [🧩 技能](https://clawhub.ai/gianni-dalerta/memory-tools) *带有本地数据库 + 嵌入的代理控制长期记忆。* (类型: Skill, 成熟度: Active, 集成方式: Gateway Skill, 许可证: N/A, Stars: ⭐0, Downloads: ~1,044)

- (2026-02-18) **Personas** [🧩 技能](https://clawhub.ai/robbyczgw-cla/personas) *按需在专用角色之间切换（节省 Token）。* (类型: Skill, 成熟度: Active, 集成方式: Gateway Skill, 许可证: N/A, Stars: ⭐9, Downloads: ~2,222)

- (2026-02-18) **OpenClaw Agent Optimize** [🧩 技能](https://clawhub.ai/phenomenoner/openclaw-agent-optimize) *路由/上下文/记忆/保障措施的优化手册。* (类型: Skill, 成熟度: Active, 集成方式: Local-only, 许可证: N/A, Stars: ⭐4, Downloads: ~1.6k)

- (2026-02-18) **Cron & Scheduling** [🧩 技能](https://clawhub.ai/gitgoodordietrying/cron-scheduling) *用于安全定期自动化的 Cron + systemd 定时器模式。* (类型: Skill, 成熟度: Active, 集成方式: Local-only, 许可证: N/A, Stars: —)

### 4.6 多模态 / 语音 / 媒体 (ClawHub)

- (2026-02-18) **Voice Transcribe** [🧩 技能](https://clawhub.ai/darinkishore/voice-transcribe) *使用 OpenAI 转录模型转录音频文件。* (类型: Skill, 成熟度: Active, 集成方式: Service, 许可证: N/A, Stars: —)

- (2026-02-18) **ElevenLabs Agents** [🧩 技能](https://clawhub.ai/PennyroyalTea/elevenlabs-agents) *创建/管理 ElevenLabs 对话式语音代理。* (类型: Skill, 成熟度: Active, 集成方式: Service, 许可证: N/A, Stars: ⭐1, Downloads: ~951)

- (2026-02-18) **Google Gemini Media** [🧩 技能](https://clawhub.ai/Xsir0/google-gemini-media) *通过 Gemini API 的多模态工作流（图像/视频/TTS）。* (类型: Skill, 成熟度: Active, 集成方式: Service, 许可证: N/A, Stars: —)

- (2026-02-18) **Gemini Computer Use** [🧩 技能](https://clawhub.ai/am-will/gemini-computer-use) *基于 Playwright 的“计算机使用”代理循环模式。* (类型: Skill, 成熟度: Active, 集成方式: Gateway Skill, 许可证: N/A, Stars: —)

### 4.7 杂项 / 生态系统技能 (ClawHub)

- (2026-02-18) **Asana** [🧩 技能](https://www.clawhub.ai/k0nkupa/asana) *Asana 任务/项目交互技能。* (类型: Skill, 成熟度: Active, 集成方式: Service, 许可证: N/A, Stars: ⭐0, Downloads: ~163)

- (2026-02-18) **xAI Plus** [🧩 技能](https://clawhub.ai/mischasigtermans/xai-plus) *搜索 X 并通过 xAI API 与 Grok 模型聊天。* (类型: Skill, 成熟度: Active, 集成方式: Service, 许可证: N/A, Stars: ⭐0, Downloads: ~409)

- (2026-02-18) **X Algorithm Mastery** [🧩 技能](https://clawhub.ai/lxgicstudios/x-mastery) *X 互动启发式和发帖手册。* (类型: Skill, 成熟度: Active, 集成方式: Local-only, 许可证: N/A, Stars: ⭐1, Downloads: ~160)

- (2026-02-18) **X Articles** [🧩 技能](https://clawhub.ai/NextFrontierBuilds/x-articles) *使用自动化模式发布 X 文章。* (类型: Skill, 成熟度: Active, 集成方式: Gateway Skill, 许可证: N/A, Stars: —)

- (2026-02-18) **diagram-gen** [🧩 技能](https://clawhub.ai/lxgicstudios/diagram-gen) *从结构化提示生成图表。* (类型: Skill, 成熟度: Active, 集成方式: Gateway Skill, 许可证: N/A, Stars: —)

- (2026-02-18) **Mixpost** [🧩 技能](https://clawhub.ai/lao9s/mixpost) *自托管社交调度集成。* (类型: Skill, 成熟度: Active, 集成方式: Service, 许可证: N/A, Stars: —)

- (2026-02-18) **ClawNet** [🧩 技能](https://clawhub.ai/dendisuhubdy/clawnet) *用于 OpenClaw 机器人的基于 QUIC 的 P2P 发现 + NAT 穿透。* (类型: Skill, 成熟度: Active, 集成方式: Service, 许可证: N/A, Stars: —)

- (2026-02-18) **SwitchBot OpenAPI** [🧩 技能](https://clawhub.ai/switchbot-dev/switchbot-cloudapi) *通过官方 OpenAPI 控制 SwitchBot 设备。* (类型: Skill, 成熟度: Active, 集成方式: Service, 许可证: N/A, Stars: —)

- (2026-02-18) **Botcoin** [🧩 技能](https://clawhub.ai/adamkristopher/botcoin) *益智游戏代币工作流（高风险领域；请仔细审查）。* (类型: Skill, 成熟度: Experimental, 集成方式: Service, 许可证: N/A, Stars: —)

- (2026-02-18) **GPT** [🧩 技能](https://clawhub.ai/0xterrybit/gpt) *OpenAI API 包装器 (聊天/图像/嵌入)。* (类型: Skill, 成熟度: Active, 集成方式: Service, 许可证: N/A, Stars: —)

- (2026-02-18) **Testosterone Optimization** [🧩 技能](https://clawhub.ai/jhillin8/testosterone-optimization) *生活方式追踪手册。* (类型: Skill, 成熟度: Experimental, 集成方式: Local-only, 许可证: N/A, Stars: ⭐0, Downloads: ~392)

- (2026-02-18) **x402-client** [🧩 技能](https://clawhub.ai/Samoppakiks/x402-client) *ClawHub 技能页面（审查发布者 + 范围）。* (类型: Skill, 成熟度: Experimental, 集成方式: Service, 许可证: N/A, Stars: —)

- (2026-02-18) **localrank-agent-skills** [🧩 技能](https://clawhub.ai/kn7f8mvt8194cgs6fa4knhrajs807s3a/localrank-agent-skills) *ClawHub 技能条目（验证来源）。* (类型: Skill, 成熟度: Experimental, 集成方式: Service, 许可证: N/A, Stars: —)

---

## 5. 真实应用案例

### 公开撰文 / 部署笔记 (精选)

- (2026-02-18) **HN: 容器化 OpenClaw 使用 (cron + VNC browser)** [📰 文章](https://news.ycombinator.com/item?id=47004312) *示例部署模式：隔离容器 + VNC + 共享文件夹 + cron 作业。* (类型: Real-world Usage, 成熟度: Active, 集成方式: Container, 许可证: N/A, Stars: —)

- (2026-02-18) **Wired: 企业禁令 / 安全担忧** [📰 文章](https://www.wired.com/story/openclaw-banned-by-tech-companies-as-security-concerns-mount) *真实组织对代理自治和供应链风险的政策响应。* (类型: Real-world Usage, 成熟度: Active, 集成方式: Policy, 许可证: N/A, Stars: —)

- (2026-02-18) **The Verge: 市场中的恶意技能** [📰 文章](https://www.theverge.com/news/874011/openclaw-ai-skill-clawhub-extensions-security-nightmare) *市场威胁面：恶意技能载荷和不安全指令。* (类型: Security, 成熟度: Active, 集成方式: Policy, 许可证: N/A, Stars: —)

---

## 6. 安全

### 权威安全构件

- (2026-02-18) **OpenClaw Trust** [💻 仓库](https://github.com/openclaw/trust) [🌐 网站](https://trust.openclaw.ai) *威胁模型 + 缓解措施；基于 MITRE ATLAS。* (类型: Security, 成熟度: Active, 集成方式: Docs, 许可证: —, Stars: ~116)

- (2026-02-18) **OpenClaw × VirusTotal (公告)** [🌐 网站](https://openclaw.ai/blog/virustotal-partnership) *官方扫描合作伙伴关系（技能/构件扫描）。* (类型: Security, 成熟度: Active, 集成方式: Service, 许可证: —, Stars: —)

### 加固安装 / 隔离模式 (官方优先)

- (2026-02-18) **openclaw-ansible** [💻 仓库](https://github.com/openclaw/openclaw-ansible) *强调网络隔离和主机加固的自动化。* (类型: Security, 成熟度: Active, 集成方式: Host/Infra, 许可证: MIT, Stars: ~346)

### 技能审查工具 (ClawHub)

- (2026-02-18) **Skill Vetter** [🧩 技能](https://clawhub.ai/steipete/skill-vetter) *用于技能安全的偏执审查管道。* (类型: Security, 成熟度: Active, 集成方式: Gateway Skill, 许可证: N/A, Stars: ⭐7, Downloads: ~2.6k)

- (2026-02-18) **Skill Scanner** [🧩 技能](https://clawhub.ai/bvinci1-design/skill-scanner) *本地扫描和审查工作流。* (类型: Security, 成熟度: Active, 集成方式: Local-only, 许可证: N/A, Stars: ⭐5, Downloads: ~1.9k)

- (2026-02-18) **Skill Defender** [🧩 技能](https://clawhub.ai/itsclawdbro/skill-defender) *检测已安装技能中的提示注入和渗漏模式。* (类型: Security, 成熟度: Active, 集成方式: Gateway Skill, 许可证: N/A, Stars: —)

---

## 7. 部署

### 官方安装与打包

- (2026-02-18) **Install (Docs)** [📄 文档](https://docs.openclaw.ai/install) *推荐的安装程序 + 替代安装方法。* (类型: Packaging/Deploy, 成熟度: Production, 集成方式: Docs, 许可证: —, Stars: —)

- (2026-02-18) **Homebrew Tap** [💻 仓库](https://github.com/openclaw/homebrew-tap) *Brew 分发入口。* (类型: Packaging/Deploy, 成熟度: Active, 集成方式: Local-only, 许可证: —, Stars: ~27)

- (2026-02-18) **Nix Package** [💻 仓库](https://github.com/openclaw/nix-openclaw) *Nix 打包。* (类型: Packaging/Deploy, 成熟度: Active, 集成方式: Local-only, 许可证: —, Stars: ~399)

- (2026-02-18) **Ansible Hardened Install** [💻 仓库](https://github.com/openclaw/openclaw-ansible) *带加固的自动化安装。* (类型: Packaging/Deploy, 成熟度: Active, 集成方式: Host/Infra, 许可证: MIT, Stars: ~346)

---

## 8. 社区

- (2026-02-18) **openclaw (GitHub org)** [🌐 网站](https://github.com/openclaw) *核心仓库、注册表、信任模型和基础设施工具的规范组织。* (类型: Community, 成熟度: Production, 集成方式: Org, 许可证: —, Stars: —)

- (2026-02-18) **ClawHub (registry)** [🌐 网站](https://clawhub.ai) *整个生态系统使用的主要技能目录。* (类型: Community, 成熟度: Production, 集成方式: Registry, 许可证: MIT, Stars: —)

- (2026-02-18) **voice-community** [💻 仓库](https://github.com/openclaw/voice-community) *社区语音实验。* (类型: Community, 成熟度: Experimental, 集成方式: Local-only, 许可证: —, Stars: ~4)

---

## 🔁 工作流阶段 (Workflow Stages)

一个典型的 OpenClaw “生产路径”：

1. **网关部署 (Gateway deployment)**
   - 通过文档安装程序安装；选择打包路线 (Nix/Homebrew/Ansible)。
2. **通道接入 (Channel onboarding)**
   - 绑定你实际使用的通道（聊天优先的控制面）。
3. **技能发现与安装 (Skill discovery & install)**
   - 从 ClawHub 开始；仅安装经过审查的技能；优先选择 CLI 包装器和最小权限流程。
4. **技能组合 (Skill composition)**
   - 将可重复的例程移入 **Lobster** 工作流（类型化管道 + 门控）。
5. **记忆与长期上下文 (Memory & long-term context)**
   - 添加显式记忆工具（混合搜索 / 嵌入）并保持来源可审计。
6. **安全加固 (Security hardening)**
   - 应用 OpenClaw Trust 控制；隔离运行时；限制出站；扫描技能/构件。
7. **生产运维 (Production operations)**
   - 调度 (cron/systemd)、备份、升级策略、事件响应手册。

---

## 🧩 领域应用 (Domain Applications)

> 示例映射到此列表中的真实组件（技能/仓库）。

- **家庭 / 智能家居**
  - Casa (HomeKit 桥接), SwitchBot OpenAPI 技能, 通过 cron/systemd 调度。

- **生产力**
  - Notion 技能, 日历 (Apple/Google/CalDAV) 技能, 邮件工作流 (Himalaya/Workspace services)。

- **DevOps / 工程**
  - GitHub (gh CLI) 技能, Lobster 工作流, cron/systemd 定时器, 通过 Ansible 加固主机安装。

- **企业 / 治理**
  - OpenClaw Trust + 技能审查/扫描 + 隔离优先部署模式。

- **教育 / 研究**
  - Google Search grounding / MCP 技能, DeepWiki (仓库文档问答), 通过 Notion 的结构化笔记系统。

- **媒体**
  - 语音转录 + Gemini 媒体工作流。

---

## 9. 相关 Awesome 列表

- (2026-02-18) **Awesome OpenClaw (rohitg00)** [💻 仓库](https://github.com/rohitg00/awesome-openclaw) *社区策划的 OpenClaw 资源。* (类型: Related List, 成熟度: Active, 集成方式: Docs, 许可证: —, Stars: —)

- (2026-02-18) **awesome-openclaw (vincentkoc)** [💻 仓库](https://github.com/vincentkoc/awesome-openclaw) *社区列表（验证新鲜度）。* (类型: Related List, 成熟度: Active, 集成方式: Docs, 许可证: —, Stars: —)

- (2026-02-18) **awesome-claw (qhkm)** [💻 仓库](https://github.com/qhkm/awesome-claw) *社区 claw 家族列表。* (类型: Related List, 成熟度: Active, 集成方式: Docs, 许可证: —, Stars: —)

- (2026-02-18) **Awesome Agentic Labs** [💻 仓库](https://github.com/wu-yc/Awesome-Agentic-Labs) *分类体系/风格的基准参考。* (类型: Related List, 成熟度: Active, 集成方式: Docs, 许可证: —, Stars: —)

---

## 10. 贡献指南

欢迎提交 PR。请遵循上述规范。

### 提交模板 (表格)

| 字段 | 要求 |
|---|---|
| Name | **粗体** 项目/技能名称 |
| Date | `(YYYY-MM-DD)` (添加/验证时) |
| Links | 提供规范链接: Repo/Site/Docs/Paper/Video |
| Description | *≤25 字, 极简, 事实性* |
| Taxonomy | 类型 + 成熟度 + 集成方式 |
| License | 优先使用确切的 SPDX (MIT/Apache-2.0/etc); 如果未知使用 `—` |
| Stars | 使用 `~` 表示近似值; 对于技能, 注明 ClawHub stars/downloads |

### 示例行

| Date | Name | Links | Description | Type | Maturity | Integration | License | Stars |
|---|---|---|---|---|---|---|---|---|
| 2026-02-18 | **OpenClaw** | Repo / Site / Docs | *Local-first personal AI assistant.* | Assistant | Production | Gateway | MIT | ~209k |

---

## 11. 关键引用

> 与本地优先代理、工具使用、记忆和安全相关的基础阅读材料。

- (2026-02-18) **ReAct: Synergizing Reasoning and Acting in Language Models** [📝 论文](https://arxiv.org/abs/2210.03629)
- (2026-02-18) **Toolformer: Language Models Can Teach Themselves to Use Tools** [📝 论文](https://arxiv.org/abs/2302.04761)
- (2026-02-18) **Retrieval-Augmented Generation (RAG)** [📝 论文](https://arxiv.org/abs/2005.11401)
- (2026-02-18) **Generative Agents (long-lived behavior + memory patterns)** [📝 论文](https://arxiv.org/abs/2304.03442)
- (2026-02-18) **MemGPT: Towards LLMs as OS-like agents with memory tiers** [📝 论文](https://arxiv.org/abs/2310.08560)
- (2026-02-18) **Local-first Software (Ink & Switch)** [📄 文档](https://www.inkandswitch.com/local-first/)
- (2026-02-18) **MITRE ATLAS** [📄 文档](https://atlas.mitre.org)

---

## 12. Star 历史

- OpenClaw (核心) star 历史: https://star-history.com/#openclaw/openclaw&Date
- ClawHub (注册表) star 历史: https://star-history.com/#openclaw/clawhub&Date

---
