# 🦞 Awesome OpenClaw Family

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
[![Contributions Welcome](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](#-contributing)
[![License: CC0](https://img.shields.io/badge/License-CC0--1.0-lightgrey.svg)](LICENSE)
[![Stars](https://img.shields.io/github/stars/YOUR_GITHUB_USERNAME/Awesome-OpenClaw-Family?style=social)](https://github.com/YOUR_GITHUB_USERNAME/Awesome-OpenClaw-Family/stargazers)

*A rigorously curated map of the OpenClaw ecosystem: core runtime, channels, skill registry, workflow shell, security hardening, deployments, and real-world usage.*

> Give this repo a star if it helps you ship a better local-first assistant.

**Maintainer:** `@wu-yc` · **PRs welcome** · **Snapshot date:** **2026-02-18** (metrics may drift slightly after this date)

---

## 🧭 Overview

OpenClaw is a local-first personal AI assistant you run on your own devices, designed to work through the messaging channels you already use, and extended via a skill marketplace + composable workflow shell. This list focuses on **canonical** OpenClaw-family projects (official repos first), **verified** ecosystem components (skills, hardening, deployments), and **high-signal** derivatives (forks/reimplementations) that matter for production-quality local agents.

---

## 🗞️ News

- (2026-02-18) **This repo**: rewritten to “Awesome-Agentic-Labs-grade” conventions (taxonomy + uniform entries + workflow stages + domain applications).
- (2026-02-18) **OpenClaw × VirusTotal**: official partnership announced for skill and artifact scanning.
- (2026-02-17) **OpenClaw**: stable release line continues (see GitHub releases).
- (2026-02-04) **Skill marketplace risk**: public reporting highlights malicious skills and supply-chain concerns.
- (2026-01-29) **Rename**: OpenClaw introduced (formerly Moltbot / Clawdbot).

---

## 🧾 Conventions

### Taxonomy

Each entry follows:

`(YYYY-MM-DD) **Name** [📝 Paper] [💻 Repo] [🌐 Site] [📄 Docs] *≤25-word description.* (Type: ..., Maturity: ..., Integration: ..., License: ..., Stars: ...)`

**Type**
- **Assistant**: the primary local agent runtime.
- **Gateway/Control Plane**: orchestration, configuration, session control.
- **Channel**: WhatsApp/Telegram/Slack/etc connectors.
- **Skill Registry**: discovery, indexing, distribution.
- **Skill**: a callable capability package (often via ClawHub).
- **Workflow Engine**: typed pipelines / approval gates / deterministic automations.
- **Security**: threat models, scanners, hardening suites.
- **Packaging/Deploy**: installers, Nix/Homebrew, Ansible, infra modules.
- **Derivative**: forks, reimplementations, alternatives in the Claw family.

**Maturity**
- **Production**: widely used, stable interfaces, active maintenance.
- **Active**: maintained + usable, may change.
- **Beta**: functional but still evolving.
- **Experimental**: early-stage, unstable interfaces.
- **Archived**: frozen, historically useful.

**Integration**
- **Local-only**: no outbound network access by default.
- **CLI Wrapper**: wraps a local CLI tool (gh/op/etc).
- **Gateway Skill**: installed into an OpenClaw agent environment.
- **Service**: external hosted API/service involved.
- **Registry**: directory / marketplace / index.

### Links

- Prefer **official** GitHub repos and official docs/sites.
- If no canonical repo exists, provide a **GitHub search** link.
- For skills, prefer the **ClawHub skill page**; if the upstream code is ambiguous, mark it clearly.

---

## 📌 Content

- [1. Core OpenClaw (Official)](#1-core-openclaw-official)
- [2. Forks & Reimplementations](#2-forks--reimplementations)
- [3. Similar Projects & Alternatives](#3-similar-projects--alternatives)
- [4. Skills & Extensions](#4-skills--extensions)
- [5. Real-World Usages & Applications](#5-real-world-usages--applications)
- [6. Security](#6-security)
- [7. Deployment](#7-deployment)
- [8. Community](#8-community)
- [Workflow Stages](#-workflow-stages)
- [Domain Applications](#-domain-applications)
- [9. Related Awesome Lists](#9-related-awesome-lists)
- [10. Contributing](#10-contributing)
- [11. Key Citations](#11-key-citations)
- [12. Star History](#12-star-history)

---

## 1. Core OpenClaw (Official)

### Core Runtime & Docs

- (2026-02-18) **OpenClaw** [💻 Repo](https://github.com/openclaw/openclaw) [🌐 Site](https://openclaw.ai) [📄 Docs](https://docs.openclaw.ai) *Local-first personal AI assistant with multi-channel chat, skills, and workflows.* (Type: Assistant, Maturity: Production, Integration: Gateway, License: MIT, Stars: ~209k)

- (2026-02-18) **OpenClaw Install Guide** [📄 Docs](https://docs.openclaw.ai/install) *Installer + platform-specific install paths (macOS/Linux/Windows via WSL2).* (Type: Packaging/Deploy, Maturity: Production, Integration: Docs, License: —, Stars: —)

- (2026-02-18) **openclaw.ai (website repo)** [💻 Repo](https://github.com/openclaw/openclaw.ai) [🌐 Site](https://openclaw.ai) *Source for the official website and distribution entrypoints.* (Type: Gateway/Control Plane, Maturity: Active, Integration: Site, License: —, Stars: ~171)

### Skill Registry & Marketplace

- (2026-02-18) **ClawHub** [💻 Repo](https://github.com/openclaw/clawhub) [🌐 Site](https://clawhub.ai) *OpenClaw’s skill registry with fast discovery and indexing.* (Type: Skill Registry, Maturity: Production, Integration: Registry, License: MIT, Stars: ~2.3k)

- (2026-02-18) **openclaw/skills (archive)** [💻 Repo](https://github.com/openclaw/skills) *Archived historical versions of skills published to clawdhub.com.* (Type: Skill Registry, Maturity: Archived, Integration: Registry, License: MIT, Stars: ~1.1k)

### Workflow Shell

- (2026-02-18) **Lobster** [💻 Repo](https://github.com/openclaw/lobster) *Typed, local-first workflow shell: pipelines, jobs, and approval gates for agent automations.* (Type: Workflow Engine, Maturity: Active, Integration: Local-only, License: MIT, Stars: ~506)

### Security Canon

- (2026-02-18) **OpenClaw Trust** [💻 Repo](https://github.com/openclaw/trust) [🌐 Site](https://trust.openclaw.ai) *Machine-checkable threat model + mitigations mapped to MITRE ATLAS.* (Type: Security, Maturity: Active, Integration: Docs, License: —, Stars: ~116)

### Packaging & Ops (Official)

- (2026-02-18) **nix-openclaw** [💻 Repo](https://github.com/openclaw/nix-openclaw) *Nix packaging for OpenClaw.* (Type: Packaging/Deploy, Maturity: Active, Integration: Local-only, License: —, Stars: ~399)

- (2026-02-18) **openclaw-ansible** [💻 Repo](https://github.com/openclaw/openclaw-ansible) *Hardened install automation (Tailscale VPN, UFW firewall, Docker isolation).* (Type: Packaging/Deploy, Maturity: Active, Integration: Host/Infra, License: MIT, Stars: ~346)

- (2026-02-18) **homebrew-tap** [💻 Repo](https://github.com/openclaw/homebrew-tap) *Official Homebrew tap.* (Type: Packaging/Deploy, Maturity: Active, Integration: Local-only, License: —, Stars: ~27)

- (2026-02-18) **clawdinators** [💻 Repo](https://github.com/openclaw/clawdinators) *Declarative infra + NixOS modules for “CLAWTINATOR” hosts.* (Type: Packaging/Deploy, Maturity: Active, Integration: Host/Infra, License: MIT, Stars: ~109)

- (2026-02-18) **clawgo** [💻 Repo](https://github.com/openclaw/clawgo) *Go implementation of a Clawd node.* (Type: Derivative, Maturity: Experimental, Integration: Local-only, License: MIT, Stars: ~33)

### Official Side Projects

- (2026-02-18) **Casa** [💻 Repo](https://github.com/openclaw/casa) *Local-only HomeKit bridge (REST API + CLI) for automation/agents on macOS.* (Type: Channel, Maturity: Experimental, Integration: Local-only, License: —, Stars: ~24)

- (2026-02-18) **butter.bot** [💻 Repo](https://github.com/openclaw/butter.bot) [🌐 Site](https://butter.bot) *Tiny official side project site repo (HTML).* (Type: Community, Maturity: Experimental, Integration: Site, License: MIT, Stars: ~7)

- (2026-02-18) **voice-community** [💻 Repo](https://github.com/openclaw/voice-community) *Community scratch space for voice-related experiments.* (Type: Community, Maturity: Experimental, Integration: Local-only, License: —, Stars: ~4)

- (2026-02-18) **barnacle** [💻 Repo](https://github.com/openclaw/barnacle) *Small utility bot (“sticks around”).* (Type: Community, Maturity: Experimental, Integration: Bot, License: —, Stars: ~14)

---

## 2. Forks & Reimplementations

> Only real, discoverable, high-signal derivatives. Official OpenClaw remains canonical.

- (2026-02-18) **NanoClaw** [💻 Repo](https://github.com/qwibitai/nanoclaw) *Container-first lightweight alternative focused on security and multi-channel usage.* (Type: Derivative, Maturity: Active, Integration: Container, License: MIT, Stars: ~8.9k)

- (2026-02-18) **nanobot** [💻 Repo](https://github.com/HKUDS/nanobot) *Ultra-lightweight OpenClaw-inspired assistant (small, auditable core).* (Type: Derivative, Maturity: Active, Integration: Local-only, License: MIT, Stars: ~20.8k)

- (2026-02-18) **PicoClaw** [💻 Repo](https://github.com/sipeed/picoclaw) [🌐 Site](https://picoclaw.ai) *Go-based ultra-light assistant aimed at low-resource hardware.* (Type: Derivative, Maturity: Active, Integration: Local-only, License: MIT, Stars: ~8.4k)

- (2026-02-18) **ZeroClaw** [💻 Repo](https://github.com/zeroclaw-labs/zeroclaw) [🌐 Site](https://zeroclaw.org) *Rust-based “agent runtime kernel” style re-think of the Claw family.* (Type: Derivative, Maturity: Active, Integration: Local-only, License: —, Stars: ~13.6k)

- (2026-02-18) **femtoclaw** [💻 Repo](https://github.com/mcotdev/femtoclaw) *Tiny Rust-based OpenClaw variant (minimal footprint).* (Type: Derivative, Maturity: Experimental, Integration: Local-only, License: MIT, Stars: ~4)

- (2026-02-18) **IronClaw (NEAR AI)** [💻 Repo](https://github.com/nearai/ironclaw) *Rust reimplementation emphasizing sandboxing and capability-style controls.* (Type: Derivative, Maturity: Active, Integration: Local-only, License: —, Stars: —)

---

## 3. Similar Projects & Alternatives

> Adjacent building blocks and ecosystem bridges commonly used around OpenClaw deployments.

- (2026-02-18) **skills.sh (ecosystem)** [🌐 Site](https://skills.sh) *Independent skill registry ecosystem referenced by ClawHub tooling.* (Type: Skill Registry, Maturity: Active, Integration: Registry, License: —, Stars: —)

- (2026-02-18) **MITRE ATLAS** [🌐 Site](https://atlas.mitre.org) *Adversarial threat knowledge base for AI-enabled systems; used in OpenClaw Trust mapping.* (Type: Security, Maturity: Production, Integration: Reference, License: —, Stars: —)

---

## 4. Skills & Extensions

> A curated snapshot of **high-signal** ClawHub skills (official + popular + security-relevant).
>
> **Note on metrics:** For skills, “Stars” and “Downloads” refer to **ClawHub** counters when visible on the skill page.

### 4.1 Core / Maintainer Skills (ClawHub)

- (2026-02-18) **Notion** [🧩 Skill](https://clawhub.ai/steipete/notion) *Notion API helper for pages/databases/blocks.* (Type: Skill, Maturity: Active, Integration: Gateway Skill, License: N/A, Stars: ⭐28, Downloads: ~9.5k)

- (2026-02-18) **Weather** [🧩 Skill](https://clawhub.ai/steipete/weather) *Weather + forecasts without API keys.* (Type: Skill, Maturity: Active, Integration: CLI Wrapper, License: N/A, Stars: ⭐25, Downloads: ~15.6k)

- (2026-02-18) **1Password** [🧩 Skill](https://clawhub.ai/steipete/1password) *1Password CLI (`op`) usage for safe secret injection.* (Type: Skill, Maturity: Active, Integration: CLI Wrapper, License: N/A, Stars: ⭐10, Downloads: ~4k)

- (2026-02-18) **Spotify Player** [🧩 Skill](https://clawhub.ai/steipete/spotify-player) *Terminal Spotify playback/search via CLI.* (Type: Skill, Maturity: Active, Integration: CLI Wrapper, License: N/A, Stars: ⭐6, Downloads: ~4.5k)

- (2026-02-18) **GitHub (gh CLI)** [🧩 Skill](https://clawhub.ai/steipete/github) *Use `gh` for PRs, issues, and CI runs.* (Type: Skill, Maturity: Active, Integration: CLI Wrapper, License: N/A, Stars: —)

- (2026-02-18) **Clawdhub CLI** [🧩 Skill](https://clawhub.ai/steipete/clawdhub) *Search/install/update/publish skills via ClawdHub.* (Type: Skill, Maturity: Active, Integration: CLI Wrapper, License: N/A, Stars: —)

- (2026-02-18) **Apple Reminders** [🧩 Skill](https://clawhub.ai/steipete/apple-reminders) *Manage Apple Reminders on macOS via CLI.* (Type: Skill, Maturity: Active, Integration: CLI Wrapper, License: N/A, Stars: —)

- (2026-02-18) **Peekaboo** [🧩 Skill](https://clawhub.ai/steipete/peekaboo) *Capture/automate macOS UI using a local CLI.* (Type: Skill, Maturity: Active, Integration: CLI Wrapper, License: N/A, Stars: —)

- (2026-02-18) **OpenAI Image Gen** [🧩 Skill](https://clawhub.ai/steipete/openai-image-gen) *Batch generate images via OpenAI Images API with a local gallery.* (Type: Skill, Maturity: Active, Integration: Service, License: N/A, Stars: —)

- (2026-02-18) **Blogwatcher** [🧩 Skill](https://clawhub.ai/steipete/blogwatcher) *Monitor RSS/Atom feeds for updates via CLI.* (Type: Skill, Maturity: Active, Integration: CLI Wrapper, License: N/A, Stars: —)

- (2026-02-18) **Gog (Google Workspace CLI)** [🧩 Skill](https://clawhub.ai/steipete/gog) *Google Workspace CLI workflows (Gmail/Calendar/Drive/etc).* (Type: Skill, Maturity: Active, Integration: CLI Wrapper, License: N/A, Stars: —)

- (2026-02-18) **Things (macOS)** [🧩 Skill](https://www.clawhub.ai/steipete/things-mac) *Manage Things 3 tasks/projects via CLI + local DB.* (Type: Skill, Maturity: Active, Integration: CLI Wrapper, License: N/A, Stars: —)

### 4.2 Popular Utility Skills (ClawHub)

- (2026-02-18) **Ontology** [🧩 Skill](https://clawhub.ai/oswalpalash/ontology) *Structured ontology creation + transformations for agent knowledge.* (Type: Skill, Maturity: Active, Integration: Gateway Skill, License: N/A, Stars: ⭐19, Downloads: ~17.3k)

- (2026-02-18) **Google Slides** [🧩 Skill](https://clawhub.ai/byungkyu/google-slides) *Create and edit Google Slides via managed OAuth gateway.* (Type: Skill, Maturity: Active, Integration: Service, License: N/A, Stars: ⭐10, Downloads: ~7.2k)

- (2026-02-18) **Apple Calendar** [🧩 Skill](https://clawhub.ai/tyler6204/apple-calendar) *CRUD Calendar.app events on macOS via scripts.* (Type: Skill, Maturity: Active, Integration: CLI Wrapper, License: N/A, Stars: ⭐7, Downloads: ~1.5k)

- (2026-02-18) **Apple Calendar CLI** [🧩 Skill](https://clawhub.ai/joargp/accli) *Alternative Apple Calendar CLI instruction set.* (Type: Skill, Maturity: Active, Integration: CLI Wrapper, License: N/A, Stars: —)

- (2026-02-18) **Caldav Calendar** [🧩 Skill](https://clawhub.ai/Asleep123/caldav-calendar) *CalDAV sync/query via vdirsyncer + khal.* (Type: Skill, Maturity: Active, Integration: CLI Wrapper, License: N/A, Stars: —)

- (2026-02-18) **Google Calendar (gcalcli)** [🧩 Skill](https://clawhub.ai/lstpsche/gcalcli-calendar) *Low-call Google Calendar workflows via gcalcli.* (Type: Skill, Maturity: Active, Integration: CLI Wrapper, License: N/A, Stars: —)

- (2026-02-18) **Google Calendar (API)** [🧩 Skill](https://clawhub.ai/AdrianMiller99/google-calendar) *Programmatic Google Calendar via API.* (Type: Skill, Maturity: Active, Integration: Service, License: N/A, Stars: —)

- (2026-02-18) **Calendar (generic)** [🧩 Skill](https://clawhub.ai/0xterrybit/calendar) *Calendar management and scheduling.* (Type: Skill, Maturity: Active, Integration: Service, License: N/A, Stars: —)

- (2026-02-18) **Gmail Agent** [🧩 Skill](https://clawhub.ai/r39132/gmail-agent) *Summarize unread Gmail; audit labels; purge spam/trash.* (Type: Skill, Maturity: Active, Integration: Service, License: N/A, Stars: —)

- (2026-02-18) **Clawemail (Google Workspace service)** [🧩 Skill](https://clawhub.ai/cto1/clawemail) *Workspace operations (Gmail/Drive/Docs/Sheets/Calendar) via service.* (Type: Skill, Maturity: Active, Integration: Service, License: N/A, Stars: —)

- (2026-02-18) **Himalaya** [🧩 Skill](https://clawhub.ai/skills/himalaya) *Terminal email via IMAP/SMTP (himalaya CLI).* (Type: Skill, Maturity: Active, Integration: CLI Wrapper, License: N/A, Stars: —)

- (2026-02-18) **React Email Skills** [🧩 Skill](https://clawhub.ai/christina-de-martinez/react-email-skills) *Generate responsive HTML emails with React Email.* (Type: Skill, Maturity: Active, Integration: Gateway Skill, License: N/A, Stars: —)

- (2026-02-18) **Clippy (Microsoft 365 CLI)** [🧩 Skill](https://clawhub.ai/foeken/clippy) *Outlook/M365 email + calendar management via CLI.* (Type: Skill, Maturity: Active, Integration: CLI Wrapper, License: N/A, Stars: —)

### 4.3 Security, Vetting, Governance (ClawHub)

- (2026-02-18) **Skill Vetter** [🧩 Skill](https://clawhub.ai/steipete/skill-vetter) *Automated review pipeline for suspicious skill patterns.* (Type: Skill, Maturity: Active, Integration: Gateway Skill, License: N/A, Stars: ⭐7, Downloads: ~2.6k)

- (2026-02-18) **Skill Scanner** [🧩 Skill](https://clawhub.ai/bvinci1-design/skill-scanner) *Local static scanner for malicious patterns with a UI.* (Type: Skill, Maturity: Active, Integration: Local-only, License: N/A, Stars: ⭐5, Downloads: ~1.9k)

- (2026-02-18) **AI Skill Scanner** [🧩 Skill](https://clawhub.ai/HugoSbl/ai-skill-scanner) *Scan skills for vulnerabilities and suspicious patterns.* (Type: Skill, Maturity: Active, Integration: Gateway Skill, License: N/A, Stars: —)

- (2026-02-18) **Skill Defender** [🧩 Skill](https://clawhub.ai/itsclawdbro/skill-defender) *Scan installed skills for prompt injection, exfiltration, backdoors.* (Type: Skill, Maturity: Active, Integration: Gateway Skill, License: N/A, Stars: —)

- (2026-02-18) **Sammā Suit** [🧩 Skill](https://clawhub.ai/OneZeroEight-ai/samma-suit) *Governance layers: budgets, permissions, audit logs, kill switch, vetting.* (Type: Skill, Maturity: Active, Integration: Gateway Skill, License: N/A, Stars: —)

### 4.4 Research, Web, and Browsing (ClawHub)

- (2026-02-18) **Google Search (grounding)** [🧩 Skill](https://clawhub.ai/Shaharsha/google-search-grounding) *Web search via Gemini Search Grounding + fallback APIs.* (Type: Skill, Maturity: Active, Integration: Service, License: N/A, Stars: —)

- (2026-02-18) **MCP Skill** [🧩 Skill](https://clawhub.ai/simlocker/mcp-skill) *Wrap an MCP server for web search/deep research/crawling/company research.* (Type: Skill, Maturity: Active, Integration: Service, License: N/A, Stars: —)

- (2026-02-18) **Fastest Browser Use** [🧩 Skill](https://clawhub.ai/rknoche6/fast-browser-use) *High-performance browser automation for scraping and DOM extraction.* (Type: Skill, Maturity: Active, Integration: Gateway Skill, License: N/A, Stars: —)

- (2026-02-18) **Agent Browser (v3)** [🧩 Skill](https://clawhub.ai/tekkenKK/agent-browser-3) *Browser automation instructions for web testing/forms/screenshots.* (Type: Skill, Maturity: Active, Integration: Gateway Skill, License: N/A, Stars: —)

- (2026-02-18) **Agent Browser (Clawdbot)** [🧩 Skill](https://clawhub.ai/MaTriXy/agent-browser-clawdbot) *Instruction-only wrapper for agent-browser CLI.* (Type: Skill, Maturity: Active, Integration: CLI Wrapper, License: N/A, Stars: —)

- (2026-02-18) **DeepWiki** [🧩 Skill](https://clawhub.ai/arun-8687/deepwiki) *Query a DeepWiki MCP server for GitHub repo docs and Q&A.* (Type: Skill, Maturity: Active, Integration: Service, License: N/A, Stars: —)

- (2026-02-18) **Skills.sh Search** [🧩 Skill](https://clawhub.ai/TheSethRose/skills-search) *Search skills.sh registry from CLI.* (Type: Skill, Maturity: Active, Integration: CLI Wrapper, License: N/A, Stars: ⭐3, Downloads: ~2k)

### 4.5 Memory, Personas, and Agent Ops (ClawHub)

- (2026-02-18) **Memory Tools** [🧩 Skill](https://clawhub.ai/gianni-dalerta/memory-tools) *Agent-controlled long-term memory with local DB + embeddings.* (Type: Skill, Maturity: Active, Integration: Gateway Skill, License: N/A, Stars: ⭐0, Downloads: ~1,044)

- (2026-02-18) **Personas** [🧩 Skill](https://clawhub.ai/robbyczgw-cla/personas) *Switch among specialized personas on demand (token-efficient).* (Type: Skill, Maturity: Active, Integration: Gateway Skill, License: N/A, Stars: ⭐9, Downloads: ~2,222)

- (2026-02-18) **OpenClaw Agent Optimize** [🧩 Skill](https://clawhub.ai/phenomenoner/openclaw-agent-optimize) *Optimization playbook for routing/context/memory/safeguards.* (Type: Skill, Maturity: Active, Integration: Local-only, License: N/A, Stars: ⭐4, Downloads: ~1.6k)

- (2026-02-18) **Cron & Scheduling** [🧩 Skill](https://clawhub.ai/gitgoodordietrying/cron-scheduling) *Cron + systemd timers patterns for safe recurring automations.* (Type: Skill, Maturity: Active, Integration: Local-only, License: N/A, Stars: —)

### 4.6 Multimodal / Voice / Media (ClawHub)

- (2026-02-18) **Voice Transcribe** [🧩 Skill](https://clawhub.ai/darinkishore/voice-transcribe) *Transcribe audio files using OpenAI transcription models.* (Type: Skill, Maturity: Active, Integration: Service, License: N/A, Stars: —)

- (2026-02-18) **ElevenLabs Agents** [🧩 Skill](https://clawhub.ai/PennyroyalTea/elevenlabs-agents) *Create/manage ElevenLabs conversational voice agents.* (Type: Skill, Maturity: Active, Integration: Service, License: N/A, Stars: ⭐1, Downloads: ~951)

- (2026-02-18) **Google Gemini Media** [🧩 Skill](https://clawhub.ai/Xsir0/google-gemini-media) *Multimodal workflows (image/video/TTS) via Gemini API.* (Type: Skill, Maturity: Active, Integration: Service, License: N/A, Stars: —)

- (2026-02-18) **Gemini Computer Use** [🧩 Skill](https://clawhub.ai/am-will/gemini-computer-use) *Playwright-based “computer use” agent loop patterns.* (Type: Skill, Maturity: Active, Integration: Gateway Skill, License: N/A, Stars: —)

### 4.7 Misc / Ecosystem Skills (ClawHub)

- (2026-02-18) **Asana** [🧩 Skill](https://www.clawhub.ai/k0nkupa/asana) *Asana task/project interaction skill.* (Type: Skill, Maturity: Active, Integration: Service, License: N/A, Stars: ⭐0, Downloads: ~163)

- (2026-02-18) **xAI Plus** [🧩 Skill](https://clawhub.ai/mischasigtermans/xai-plus) *Search X and chat with Grok models via xAI API.* (Type: Skill, Maturity: Active, Integration: Service, License: N/A, Stars: ⭐0, Downloads: ~409)

- (2026-02-18) **X Algorithm Mastery** [🧩 Skill](https://clawhub.ai/lxgicstudios/x-mastery) *X engagement heuristics and posting playbook.* (Type: Skill, Maturity: Active, Integration: Local-only, License: N/A, Stars: ⭐1, Downloads: ~160)

- (2026-02-18) **X Articles** [🧩 Skill](https://clawhub.ai/NextFrontierBuilds/x-articles) *Publish X Articles with automation patterns.* (Type: Skill, Maturity: Active, Integration: Gateway Skill, License: N/A, Stars: —)

- (2026-02-18) **diagram-gen** [🧩 Skill](https://clawhub.ai/lxgicstudios/diagram-gen) *Generate diagrams from structured prompts.* (Type: Skill, Maturity: Active, Integration: Gateway Skill, License: N/A, Stars: —)

- (2026-02-18) **Mixpost** [🧩 Skill](https://clawhub.ai/lao9s/mixpost) *Self-hosted social scheduling integration.* (Type: Skill, Maturity: Active, Integration: Service, License: N/A, Stars: —)

- (2026-02-18) **ClawNet** [🧩 Skill](https://clawhub.ai/dendisuhubdy/clawnet) *QUIC-based P2P discovery + NAT traversal for OpenClaw bots.* (Type: Skill, Maturity: Active, Integration: Service, License: N/A, Stars: —)

- (2026-02-18) **SwitchBot OpenAPI** [🧩 Skill](https://clawhub.ai/switchbot-dev/switchbot-cloudapi) *Control SwitchBot devices via official OpenAPI.* (Type: Skill, Maturity: Active, Integration: Service, License: N/A, Stars: —)

- (2026-02-18) **Botcoin** [🧩 Skill](https://clawhub.ai/adamkristopher/botcoin) *Puzzle-game token workflow (high-risk domain; review carefully).* (Type: Skill, Maturity: Experimental, Integration: Service, License: N/A, Stars: —)

- (2026-02-18) **GPT** [🧩 Skill](https://clawhub.ai/0xterrybit/gpt) *OpenAI API wrapper (chat/images/embeddings).* (Type: Skill, Maturity: Active, Integration: Service, License: N/A, Stars: —)

- (2026-02-18) **Testosterone Optimization** [🧩 Skill](https://clawhub.ai/jhillin8/testosterone-optimization) *Lifestyle tracking playbook.* (Type: Skill, Maturity: Experimental, Integration: Local-only, License: N/A, Stars: ⭐0, Downloads: ~392)

- (2026-02-18) **x402-client** [🧩 Skill](https://clawhub.ai/Samoppakiks/x402-client) *ClawHub skill page (review publisher + scope).* (Type: Skill, Maturity: Experimental, Integration: Service, License: N/A, Stars: —)

- (2026-02-18) **localrank-agent-skills** [🧩 Skill](https://clawhub.ai/kn7f8mvt8194cgs6fa4knhrajs807s3a/localrank-agent-skills) *ClawHub skill entry (verify provenance).* (Type: Skill, Maturity: Experimental, Integration: Service, License: N/A, Stars: —)

---

## 5. Real-World Usages & Applications

### Public Write-ups / Deploy Notes (Selected)

- (2026-02-18) **HN: containerized OpenClaw usage (cron + VNC browser)** [📰 Write-up](https://news.ycombinator.com/item?id=47004312) *Example deployment pattern: isolated container + VNC + shared folder + cron jobs.* (Type: Real-world Usage, Maturity: Active, Integration: Container, License: N/A, Stars: —)

- (2026-02-18) **Wired: enterprise bans / security concerns** [📰 Write-up](https://www.wired.com/story/openclaw-banned-by-tech-companies-as-security-concerns-mount) *Real org policy response to agent autonomy and supply-chain risk.* (Type: Real-world Usage, Maturity: Active, Integration: Policy, License: N/A, Stars: —)

- (2026-02-18) **The Verge: malicious skills in the marketplace** [📰 Write-up](https://www.theverge.com/news/874011/openclaw-ai-skill-clawhub-extensions-security-nightmare) *Marketplace threat surface: malicious skill payloads and unsafe instructions.* (Type: Security, Maturity: Active, Integration: Policy, License: N/A, Stars: —)

---

## 6. Security

### Canonical Security Artifacts

- (2026-02-18) **OpenClaw Trust** [💻 Repo](https://github.com/openclaw/trust) [🌐 Site](https://trust.openclaw.ai) *Threat model + mitigations; grounded in MITRE ATLAS.* (Type: Security, Maturity: Active, Integration: Docs, License: —, Stars: ~116)

- (2026-02-18) **OpenClaw × VirusTotal (announcement)** [🌐 Site](https://openclaw.ai/blog/virustotal-partnership) *Official scanning partnership (skill/artifact scanning).* (Type: Security, Maturity: Active, Integration: Service, License: —, Stars: —)

### Hardened Install / Isolation Patterns (Official-first)

- (2026-02-18) **openclaw-ansible** [💻 Repo](https://github.com/openclaw/openclaw-ansible) *Automation emphasizing network isolation and host hardening.* (Type: Security, Maturity: Active, Integration: Host/Infra, License: MIT, Stars: ~346)

### Skill Vetting Tooling (ClawHub)

- (2026-02-18) **Skill Vetter** [🧩 Skill](https://clawhub.ai/steipete/skill-vetter) *Opinionated vetting pipeline for skill safety.* (Type: Security, Maturity: Active, Integration: Gateway Skill, License: N/A, Stars: ⭐7, Downloads: ~2.6k)

- (2026-02-18) **Skill Scanner** [🧩 Skill](https://clawhub.ai/bvinci1-design/skill-scanner) *Local scan and review workflow.* (Type: Security, Maturity: Active, Integration: Local-only, License: N/A, Stars: ⭐5, Downloads: ~1.9k)

- (2026-02-18) **Skill Defender** [🧩 Skill](https://clawhub.ai/itsclawdbro/skill-defender) *Detect prompt injection and exfil patterns across installed skills.* (Type: Security, Maturity: Active, Integration: Gateway Skill, License: N/A, Stars: —)

---

## 7. Deployment

### Official Install & Packaging

- (2026-02-18) **Install (Docs)** [📄 Docs](https://docs.openclaw.ai/install) *Recommended installer + alternative install methods.* (Type: Packaging/Deploy, Maturity: Production, Integration: Docs, License: —, Stars: —)

- (2026-02-18) **Homebrew Tap** [💻 Repo](https://github.com/openclaw/homebrew-tap) *Brew distribution entrypoint.* (Type: Packaging/Deploy, Maturity: Active, Integration: Local-only, License: —, Stars: ~27)

- (2026-02-18) **Nix Package** [💻 Repo](https://github.com/openclaw/nix-openclaw) *Nix packaging.* (Type: Packaging/Deploy, Maturity: Active, Integration: Local-only, License: —, Stars: ~399)

- (2026-02-18) **Ansible Hardened Install** [💻 Repo](https://github.com/openclaw/openclaw-ansible) *Automated install with hardening.* (Type: Packaging/Deploy, Maturity: Active, Integration: Host/Infra, License: MIT, Stars: ~346)

---

## 8. Community

- (2026-02-18) **openclaw (GitHub org)** [🌐 Site](https://github.com/openclaw) *Canonical org for core repos, registry, trust model, and infra tools.* (Type: Community, Maturity: Production, Integration: Org, License: —, Stars: —)

- (2026-02-18) **ClawHub (registry)** [🌐 Site](https://clawhub.ai) *Primary skill directory used across the ecosystem.* (Type: Community, Maturity: Production, Integration: Registry, License: MIT, Stars: —)

- (2026-02-18) **voice-community** [💻 Repo](https://github.com/openclaw/voice-community) *Community voice experiments.* (Type: Community, Maturity: Experimental, Integration: Local-only, License: —, Stars: ~4)

---

## 🔁 Workflow Stages

A typical OpenClaw “production path”:

1. **Gateway deployment**
   - Install via docs installer; choose a packaging route (Nix/Homebrew/Ansible).
2. **Channel onboarding**
   - Bind the channels you actually use (chat-first control surface).
3. **Skill discovery & install**
   - Start from ClawHub; install only vetted skills; prefer CLI wrappers and least-privilege flows.
4. **Skill composition**
   - Move repeatable routines into **Lobster** workflows (typed pipelines + gates).
5. **Memory & long-term context**
   - Add explicit memory tooling (hybrid search / embeddings) and keep sources auditable.
6. **Security hardening**
   - Apply OpenClaw Trust controls; isolate runtime; restrict outbound; scan skills/artifacts.
7. **Production operations**
   - Scheduling (cron/systemd), backups, upgrade policy, incident response playbooks.

---

## 🧩 Domain Applications

> Examples map to real components in this list (skills/repos).

- **Home / Smart Home**
  - Casa (HomeKit bridge), SwitchBot OpenAPI skill, scheduling via cron/systemd.

- **Productivity**
  - Notion skill, calendar (Apple/Google/CalDAV) skills, email workflows (Himalaya/Workspace services).

- **DevOps / Engineering**
  - GitHub (gh CLI) skill, Lobster workflows, cron/systemd timers, hardened host installs via Ansible.

- **Enterprise / Governance**
  - OpenClaw Trust + skill vetting/scanning + isolation-first deployment patterns.

- **Education / Research**
  - Google Search grounding / MCP skill, DeepWiki (repo doc Q&A), structured note systems via Notion.

- **Media**
  - Voice transcription + Gemini media workflows.

---

## 9. Related Awesome Lists

- (2026-02-18) **Awesome OpenClaw (rohitg00)** [💻 Repo](https://github.com/rohitg00/awesome-openclaw) *Community-curated OpenClaw resources.* (Type: Related List, Maturity: Active, Integration: Docs, License: —, Stars: —)

- (2026-02-18) **awesome-openclaw (vincentkoc)** [💻 Repo](https://github.com/vincentkoc/awesome-openclaw) *Community list (verify freshness).* (Type: Related List, Maturity: Active, Integration: Docs, License: —, Stars: —)

- (2026-02-18) **awesome-claw (qhkm)** [💻 Repo](https://github.com/qhkm/awesome-claw) *Community claw-family list.* (Type: Related List, Maturity: Active, Integration: Docs, License: —, Stars: —)

- (2026-02-18) **Awesome Agentic Labs** [💻 Repo](https://github.com/wu-yc/Awesome-Agentic-Labs) *Benchmark reference for taxonomy/style.* (Type: Related List, Maturity: Active, Integration: Docs, License: —, Stars: —)

---

## 10. Contributing

PRs are welcome. Please follow the conventions above.

### Submission Template (table)

| Field | Requirement |
|---|---|
| Name | **Bold** project/skill name |
| Date | `(YYYY-MM-DD)` (when added/verified) |
| Links | Provide canonical links: Repo/Site/Docs/Paper/Video |
| Description | *≤25 words, minimal, factual* |
| Taxonomy | Type + Maturity + Integration |
| License | Prefer exact SPDX (MIT/Apache-2.0/etc); use `—` if unknown |
| Stars | Use `~` for approximate; for skills, note ClawHub stars/downloads |

### Example Row

| Date | Name | Links | Description | Type | Maturity | Integration | License | Stars |
|---|---|---|---|---|---|---|---|---|
| 2026-02-18 | **OpenClaw** | Repo / Site / Docs | *Local-first personal AI assistant.* | Assistant | Production | Gateway | MIT | ~209k |

---

## 11. Key Citations

> Foundational reads relevant to local-first agents, tool use, memory, and safety.

- (2026-02-18) **ReAct: Synergizing Reasoning and Acting in Language Models** [📝 Paper](https://arxiv.org/abs/2210.03629)
- (2026-02-18) **Toolformer: Language Models Can Teach Themselves to Use Tools** [📝 Paper](https://arxiv.org/abs/2302.04761)
- (2026-02-18) **Retrieval-Augmented Generation (RAG)** [📝 Paper](https://arxiv.org/abs/2005.11401)
- (2026-02-18) **Generative Agents (long-lived behavior + memory patterns)** [📝 Paper](https://arxiv.org/abs/2304.03442)
- (2026-02-18) **MemGPT: Towards LLMs as OS-like agents with memory tiers** [📝 Paper](https://arxiv.org/abs/2310.08560)
- (2026-02-18) **Local-first Software (Ink & Switch)** [📄 Docs](https://www.inkandswitch.com/local-first/)
- (2026-02-18) **MITRE ATLAS** [📄 Docs](https://atlas.mitre.org)

---

## 12. Star History

- OpenClaw (core) star history: https://star-history.com/#openclaw/openclaw&Date
- ClawHub (registry) star history: https://star-history.com/#openclaw/clawhub&Date

---
