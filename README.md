# Awesome OpenClaw Family 
[![Awesome](https://awesome.re/badge.svg?logo=stylelint)](https://awesome.re) [![Contributions Welcome](https://img.shields.io/badge/Contributions-welcome-Green?logo=mercadopago&logoColor=white)](../../pulls) [![GitHub Stars](https://img.shields.io/github/stars/YOUR_GITHUB_USERNAME/Awesome-OpenClaw-Family?style=social)](https://star-history.com/#YOUR_GITHUB_USERNAME/Awesome-OpenClaw-Family) [![License](https://img.shields.io/badge/License-CC0%201.0-lightgrey.svg)](LICENSE)
### The definitive curated list of the OpenClaw ecosystem (core, forks, skills, deployments, security, and community resources)

⭐ Give this repo a star if it helps you ship a better local-first assistant. ⭐

Manually curated resources around **OpenClaw** and the broader **OpenClaw family**: the official platform, the skills marketplace, forks/reimplementations, compatible tooling, hardening practices, deployment stacks, and real-world showcases.


[ Overview](#-overview) • [ News](#-news) • [ Content](#-content) • [ Contributing](#-contributing) • [ 中文](README_CN.md)

---

## 🧭 Overview

### What is the OpenClaw family?

**OpenClaw** is a local-first, self-hosted personal AI assistant / agent platform. It’s designed to live where you already communicate—**WhatsApp, Telegram, Slack, Discord, Signal, iMessage, Teams, Matrix, Zalo, WeChat**, and more—via a single **Gateway** control plane that turns each chat into an always-on, tool-using, memory-enabled assistant.

The **OpenClaw family** includes:
- The official OpenClaw core + official extensions (skills, marketplace, packaging, deployment tooling)
- Forks and reimplementations that keep compatibility (or explore new security models)
- Adjacent projects with similar “personal agent” goals
- A growing ecosystem of skills, companion apps, and deployment stacks
- Security/hardening tooling (threat modeling, scanning, sandboxing)

### Conventions

#### Taxonomy
- **Type**
  - **Core**: official platform / gateway
  - **Official-Extension**: official repos that extend core capabilities
  - **Fork** / **Reimplementation**: compatible or inspired implementations
  - **Alternative**: similar personal assistant platforms (not necessarily OpenClaw-compatible)
  - **Skill** / **Skill-Pack**: skills, bundles, catalogs, and builders
  - **Security-Tool**: hardening, auditing, scanning, threat modeling
  - **Deployment**: installers, packaging, infra templates, ops tooling
  - **Use-Case**: real-world deployments, showcases, case studies
  - **Resource**: docs, deep dives, communities, newsletters
  - **Paper**: foundational reads (agents, memory, security)
- **Maturity**
  - `Production` / `Beta` / `Experimental` / `Archived`
- **Stars**
  - Star counts are snapshots, not ranks. Always click through for the latest.

#### Entry format
- `(YYYY-MM-DD) **Name** [📝 Paper] [💻 Repo] [🌐 Site] [🎥 Video]`
- *One-line italic description.*
- `(Type: ..., Maturity: ..., License: ..., Stars: ...)`

> **Note on licenses:** Official OpenClaw repos are consistently MIT. Community skills/tools vary; when the license is not obvious from the repo header, this list marks it as **“See repo”**.

---

## 📰 News

- **[2026/02/18]** Initial “Awesome-OpenClaw-Family” release (structure + curated seed set).
- **[2026/02/18]** Added: official ecosystem map, hardening resources, and showcase-driven real-world use cases.

---

## 📌 Content

- [1. Overview / What is the OpenClaw Family](#-overview)
- [2. Core OpenClaw (official repos + docs)](#-core-openclaw-official)
- [3. Forks & Reimplementations](#-forks--reimplementations)
- [4. Similar Projects & Alternatives](#-similar-projects--alternatives)
- [5. Skills & Extensions](#-skills--extensions)
- [6. Real-World Usages & Applications](#-real-world-usages--applications)
- [7. Security, Hardening & Auditing Tools](#-security-hardening--auditing-tools)
- [8. Deployment & Infrastructure](#-deployment--infrastructure)
- [9. Community & Resources](#-community--resources)
- [10. Related Awesome Lists](#-related-awesome-lists)
- [11. Contributing](#-contributing)
- [12. Key Citations / Foundational Reads](#-key-citations--foundational-reads)

---

## 🦞 Core OpenClaw (Official)

### Core platform & docs

- (2026-02-18) **OpenClaw** [💻 Repo](https://github.com/openclaw/openclaw) [🌐 Site](https://openclaw.ai/) [🌐 Docs](https://docs.openclaw.ai/) [🌐 Showcase](https://docs.openclaw.ai/start/showcase)  
  *Local-first, self-hosted personal assistant that lives inside your existing chat apps via a single Gateway control plane.*  
  (Type: Core, Maturity: Production, License: MIT, Stars: ~208k)

- (2026-02-18) **OpenClaw Website** [💻 Repo](https://github.com/openclaw/openclaw.ai) [🌐 Site](https://openclaw.ai/)  
  *Official website + announcements (useful for ecosystem changes and security notices).*  
  (Type: Official-Extension, Maturity: Production, License: MIT, Stars: ~11)

- (2026-02-18) **Getting Started / Wizard / FAQ** [🌐 Docs](https://docs.openclaw.ai/start/getting-started) [🌐 Wizard](https://docs.openclaw.ai/start/wizard) [🌐 FAQ](https://docs.openclaw.ai/start/faq)  
  *Canonical install + onboarding flow and operational guidance.*  
  (Type: Resource, Maturity: Production, License: -, Stars: -)

### Skills, marketplace, and “batteries included”

- (2026-02-18) **ClawHub (Marketplace)** [💻 Repo](https://github.com/openclaw/clawhub) [🌐 Site](https://clawhub.ai/)  
  *Skills marketplace + discovery layer for distributing community and official skills.*  
  (Type: Official-Extension, Maturity: Production, License: MIT, Stars: ~2.0k)

- (2026-02-18) **openclaw/skills** [💻 Repo](https://github.com/openclaw/skills)  
  *Official skill archive and reference implementations; a good baseline for patterns and compatibility.*  
  (Type: Official-Extension, Maturity: Production, License: MIT, Stars: ~1.1k)

- (2026-02-18) **Lobster** [💻 Repo](https://github.com/openclaw/lobster)  
  *Typed, local-first workflow shell (“macro engine”) for composing tools/skills into resumable pipelines and approvals.*  
  (Type: Official-Extension, Maturity: Beta, License: MIT, Stars: ~503)

### Official nodes, companion components, and experiments

- (2026-02-18) **nix-openclaw** [💻 Repo](https://github.com/openclaw/nix-openclaw)  
  *Nix packaging for reproducible OpenClaw deployments (developer + server-friendly).*  
  (Type: Deployment, Maturity: Production, License: See repo, Stars: ~397)

- (2026-02-18) **homebrew-tap** [💻 Repo](https://github.com/openclaw/homebrew-tap)  
  *Homebrew formulae/tap for installing OpenClaw tooling on macOS.*  
  (Type: Deployment, Maturity: Beta, License: MIT, Stars: ~264)

- (2026-02-18) **clawgo** [💻 Repo](https://github.com/openclaw/clawgo)  
  *A Go-based node (“clawd node in go”) for extending the ecosystem and lightweight integrations.*  
  (Type: Official-Extension, Maturity: Experimental, License: MIT, Stars: ~33)

- (2026-02-18) **casa** [💻 Repo](https://github.com/openclaw/casa)  
  *“Expose your home base to OpenClaw” — a companion piece for home-network presence/integration.*  
  (Type: Official-Extension, Maturity: Experimental, License: See repo, Stars: ~24)

- (2026-02-18) **barnacle** [💻 Repo](https://github.com/openclaw/barnacle)  
  *Small utility bot that “sticks around” (useful as a minimal reference / integration target).*  
  (Type: Official-Extension, Maturity: Experimental, License: See repo, Stars: ~14)

- (2026-02-18) **butter.bot** [💻 Repo](https://github.com/openclaw/butter.bot) [🌐 Site](https://butter.bot)  
  *Companion bot endpoint + experiments.*  
  (Type: Official-Extension, Maturity: Experimental, License: MIT, Stars: ~7)

- (2026-02-18) **voice-community** [💻 Repo](https://github.com/openclaw/voice-community)  
  *Community voice experiments / reference work for speech workflows.*  
  (Type: Official-Extension, Maturity: Experimental, License: See repo, Stars: ~4)

---

## 🧬 Forks & Reimplementations

> Forks range from “drop-in compatible” to “inspired by OpenClaw”. This section focuses on projects that meaningfully contribute new architecture, security posture, or portability.

- (2026-02-18) **IronClaw** [💻 Repo](https://github.com/nearai/ironclaw)  
  *OpenClaw-inspired Rust implementation focused on privacy/security (WASM sandboxing, allowlists, prompt-injection defenses, encrypted local data).*  
  (Type: Reimplementation, Maturity: Beta, License: Apache-2.0 / MIT, Stars: ~2.3k)

- (2026-02-18) **NanoClaw** [💻 Repo](https://github.com/flakeash/nanoclaw)  
  *High-signal “small but capable” OpenClaw alternative emphasizing rapid iteration and compatibility patterns.*  
  (Type: Alternative, Maturity: Beta, License: See repo, Stars: ~9.3k)

- (2026-02-18) **nanobot** [💻 Repo](https://github.com/qwibitai/nanobot)  
  *Minimal OpenClaw-inspired assistant implementation (good for understanding core loops + building bespoke deployments).*  
  (Type: Reimplementation, Maturity: Beta, License: See repo, Stars: ~5.4k)

- (2026-02-18) **femtoclaw** [💻 Repo](https://github.com/hhy-hhy/femtoclaw)  
  *Tiny OpenClaw alternative intended as a learning-friendly reference for core abstractions.*  
  (Type: Reimplementation, Maturity: Experimental, License: See repo, Stars: ~5.7k)

- (2026-02-18) **moltis** [💻 Repo](https://github.com/aiv1961/moltis)  
  *Rust-based personal assistant focusing on agent loops, structured tasks, and local operations.*  
  (Type: Alternative, Maturity: Experimental, License: See repo, Stars: ~432)

---

## 🔁 Similar Projects & Alternatives

> This section is intentionally conservative: “similar” here means **personal assistant + automation + long-running agent behavior**. Many great agent frameworks are listed later under [Related frameworks](#-key-citations--foundational-reads).

### Adjacent “personal agent” ecosystems
- (2026-02-18) **AionUi** [💻 Repo](https://github.com/iOfficeAI/AionUi)  
  *Local-first “cowork” app with multi-agent workflows and integrations across popular coding assistants; frequently used alongside OpenClaw setups.*  
  (Type: Alternative, Maturity: Beta, License: See repo, Stars: ~16.5k)

### Companion / agent personas
- (2026-02-18) **airi** [💻 Repo](https://github.com/moeru-ai/airi)  
  *Self-hosted AI companion with voice and game integrations; adjacent to OpenClaw-style persistent assistants.*  
  (Type: Alternative, Maturity: Beta, License: See repo, Stars: ~17.5k)

---

## 🧩 Skills & Extensions

### Skill directories, catalogs, and discovery

- (2026-02-18) **ClawHub** [🌐 Site](https://clawhub.ai/) [💻 Repo](https://github.com/openclaw/clawhub)  
  *Primary skills marketplace (search/discovery + distribution).*  
  (Type: Skill-Pack, Maturity: Production, License: MIT, Stars: ~2.0k)

- (2026-02-18) **awesome-openclaw-skills** [💻 Repo](https://github.com/VoltAgent/awesome-openclaw-skills)  
  *Largest community skill collection / index (historically also tagged under “Moltbot / Clawdbot”).*  
  (Type: Skill-Pack, Maturity: Production, License: See repo, Stars: ~16.6k)

### Skill development, templates, and builders

- (2026-02-18) **refly** [💻 Repo](https://github.com/refly-ai/refly)  
  *Skill builder toolkit used for quickly scaffolding integrations and publishing to skill ecosystems.*  
  (Type: Tool, Maturity: Beta, License: See repo, Stars: ~1.3k)

- (2026-02-18) **planning-with-files** [💻 Repo](https://github.com/OthmanAdi/planning-with-files)  
  *A “persistent markdown planning” skill/workflow that pairs well with long-running agent setups.*  
  (Type: Skill, Maturity: Production, License: See repo, Stars: ~14.1k)

- (2026-02-18) **obsidian-skills** [💻 Repo](https://github.com/TimefoldAI/obsidian-skills)  
  *Bring multi-agent skills and workflows into Obsidian; useful for knowledge + assistant convergence.*  
  (Type: Skill-Pack, Maturity: Beta, License: See repo, Stars: ~10.3k)

### Memory, knowledge, and long-term context

- (2026-02-18) **memU** [💻 Repo](https://github.com/youngking1989/memU)  
  *Long-term memory layer for assistants/agents; commonly paired with OpenClaw-style deployments.*  
  (Type: Tool, Maturity: Beta, License: See repo, Stars: ~9.9k)

- (2026-02-18) **MemOS** [💻 Repo](https://github.com/MemTensor/MemOS)  
  *“Memory OS” concepts for agent systems (persistent memory scheduling/retrieval for skills).*  
  (Type: Tool, Maturity: Beta, License: See repo, Stars: ~5.6k)

### Devtools & operator skills

- (2026-02-18) **SNAG** [💻 Repo](https://github.com/am-will/snag)  
  *Screenshot-to-Markdown/text CLI (pairs well with “agent watches screen and acts” workflows).*  
  (Type: Tool, Maturity: Beta, License: MIT, Stars: ~39)

### Home & hardware

- (2026-02-18) **Home Assistant Add-on for OpenClaw** [💻 Repo](https://github.com/ngutman/openclaw-ha-addon)  
  *Run the OpenClaw gateway as a Home Assistant add-on (good for always-on home deployments).*  
  (Type: Deployment, Maturity: Beta, License: MIT, Stars: ~73)

> Tip: The OpenClaw showcase page is a goldmine for “skills people actually run” (Bambu printer control, calendar integrations, browser autopilots, etc.). Start there and backfill into this section.  
> See: [Showcase](https://docs.openclaw.ai/start/showcase)

---

## 🌍 Real-World Usages & Applications

### Curated collections

- (2026-02-18) **awesome-openclaw-usecases** [💻 Repo](https://github.com/hesamsheikh/awesome-openclaw-usecases)  
  *Community index of “what people actually built” (home, work, devops, automation, personal life).*  
  (Type: Use-Case, Maturity: Production, License: See repo, Stars: ~4.3k)

- (2026-02-18) **OpenClaw Showcase** [🌐 Site](https://docs.openclaw.ai/start/showcase)  
  *Official showcase with real deployments, links, and short writeups (Discord/X submissions).*  
  (Type: Use-Case, Maturity: Production, License: -, Stars: -)

### Architecture deep-dives & multi-agent deployments

- (2026-02-18) **Kev’s Dream Team (Orchestrated Agents Writeup)** [💻 Repo](https://github.com/adam91holt/orchestrated-ai-articles)  
  *A public multi-agent deployment writeup (heartbeats, delegation, model selection, webhooks, and ops patterns).*  
  (Type: Use-Case, Maturity: Experimental, License: See repo, Stars: ~75)

- (2026-02-18) **Clawdspace** [💻 Repo](https://github.com/adam91holt/clawdspace)  
  *Self-hosted sandboxed execution “spaces” for agents (Docker + Tailscale; audit logs; tool integration).*  
  (Type: Security-Tool, Maturity: Experimental, License: Not specified, Stars: ~33)

---

## 🛡️ Security, Hardening & Auditing Tools

- (2026-02-18) **OpenClaw Trust (Threat Model + Security Program Data)** [💻 Repo](https://github.com/openclaw/trust) [🌐 Site](https://trust.openclaw.ai/trust/threatmodel)  
  *Threat model + trust boundaries (MITRE ATLAS-aligned), plus a public contribution path for new threats.*  
  (Type: Security-Tool, Maturity: Beta, License: Not specified, Stars: ~13)

- (2026-02-18) **OpenClaw Ansible Installer (Hardened)** [💻 Repo](https://github.com/openclaw/openclaw-ansible)  
  *Automated hardened installs (Docker isolation, firewall-first posture, Tailscale VPN, fail2ban, auto-updates).*  
  (Type: Deployment, Maturity: Production, License: MIT, Stars: ~346)

- (2026-02-18) **openclaw-skills-security** [💻 Repo](https://github.com/UseAI-pro/openclaw-skills-security)  
  *Skill security tooling (lint/scan patterns for skills; helpful in CI for ClawHub-style publishing).*  
  (Type: Security-Tool, Maturity: Beta, License: See repo, Stars: ~75)

### Security references used by OpenClaw-style systems
- **MITRE ATLAS** [🌐 Site](https://atlas.mitre.org/)  
  *Adversarial tactics and techniques for AI systems (useful for threat-modeling assistants/agents).*  
  (Type: Resource, Maturity: Production, License: -, Stars: -)

---

## 🚀 Deployment & Infrastructure

- (2026-02-18) **Nix packaging for OpenClaw** [💻 Repo](https://github.com/openclaw/nix-openclaw)  
  *Reproducible deployments + easy rollbacks.*  
  (Type: Deployment, Maturity: Production, License: See repo, Stars: ~397)

- (2026-02-18) **Docker-first (recommended for isolation)** [🌐 Docs](https://docs.openclaw.ai/install/docker)  
  *Containerized installs for sandboxing tools and preventing host compromise from agent toolchains.*  
  (Type: Deployment, Maturity: Production, License: -, Stars: -)

- (2026-02-18) **Homebrew tap** [💻 Repo](https://github.com/openclaw/homebrew-tap)  
  *Fast macOS installs for local development and CLI usage.*  
  (Type: Deployment, Maturity: Beta, License: MIT, Stars: ~264)

- (2026-02-18) **Home Assistant Add-on** [💻 Repo](https://github.com/ngutman/openclaw-ha-addon)  
  *“Always-on” home gateway deployment option.*  
  (Type: Deployment, Maturity: Beta, License: MIT, Stars: ~73)

---

## 🤝 Community & Resources

### Official
- **Discord** [🌐 Site](https://discord.gg/clawd)  
  (Type: Community, Maturity: Production)
- **GitHub Discussions** [🌐 Site](https://github.com/openclaw/openclaw/discussions)  
  (Type: Community, Maturity: Production)
- **Showcase submission flow** [🌐 Site](https://docs.openclaw.ai/start/showcase)  
  (Type: Resource, Maturity: Production)

### Community translations & mirrors
- **Traditional Chinese docs mirror (community)** [🌐 Site](https://claw-tw.jackle.pro/start/showcase)  
  (Type: Resource, Maturity: Beta)

---

## 📚 Related Awesome Lists

- **Awesome Agentic Labs** [💻 Repo](https://github.com/wu-yc/Awesome-Agentic-Labs)  
  *Gold-standard formatting reference for this list style.*  
  (Type: Resource, Maturity: Production, License: MIT)

- **awesome-openclaw-skills** [💻 Repo](https://github.com/VoltAgent/awesome-openclaw-skills)  
  *Skill-focused companion list.*  
  (Type: Skill-Pack, Maturity: Production, License: See repo)

- **awesome-openclaw-usecases** [💻 Repo](https://github.com/hesamsheikh/awesome-openclaw-usecases)  
  *Use-case focused companion list.*  
  (Type: Use-Case, Maturity: Production, License: See repo)

---

## 🙌 Contributing

PRs are welcome — especially for:
- High-quality, actively maintained skills (with screenshots or small demos)
- Production deployments (what hardware, what channels, how it’s secured)
- Security tooling (sandboxing, scanners, policy engines, audit workflows)
- Verified tutorials (with reproducible steps)

### Add an entry (format)

Please keep entries:
- **Verified** (link works, not spam, not obviously abandoned unless historically important)
- **Minimal** (one-line italic description; no marketing fluff)
- **Tagged** (Type + Maturity + License + Stars when applicable)

Use this row template (same as the reference repo):

| YYYY-MM-DD | [Paper Title](paper_link) | System/Agent | L2 | One-line description. | [GitHub](repo_link) |
|:--:|:--|:--:|:--:|:--|:--:|
| 2026-02-18 | [OpenClaw Trust](https://github.com/openclaw/trust) | Security-Tool | - | Threat model + trust boundaries for OpenClaw (MITRE ATLAS aligned). | [GitHub](https://github.com/openclaw/trust) |

---

## 🧠 Key Citations / Foundational Reads

> These are “foundation stones” for anyone building OpenClaw-class assistants: tool use, memory, multi-agent orchestration, and security.

### Tool use & agent reasoning
- (2022-10-??) **ReAct: Synergizing Reasoning and Acting in Language Models** [📝 Paper](https://arxiv.org/abs/2210.03629) [💻 Repo](https://github.com/ysymyth/ReAct)  
  *Reason+act loops for tool use; a conceptual ancestor of many agent frameworks.*  
  (Type: Paper, Autonomy: -)

- (2023-02-??) **Toolformer: Language Models Can Teach Themselves to Use Tools** [📝 Paper](https://arxiv.org/abs/2302.04761)  
  *Learning tool-use patterns via self-supervision.*  
  (Type: Paper, Autonomy: -)

### Memory & long-running agents
- (2023-04-??) **Generative Agents: Interactive Simulacra of Human Behavior** [📝 Paper](https://arxiv.org/abs/2304.03442)  
  *Memory + reflection for long-horizon agent behavior.*  
  (Type: Paper, Autonomy: -)

- (2023-10-??) **MemGPT: Towards LLMs as Operating Systems** [📝 Paper](https://arxiv.org/abs/2310.08560) [💻 Repo](https://github.com/cpacker/MemGPT)  
  *Explicit memory hierarchy + retrieval for persistent assistants.*  
  (Type: Paper, Autonomy: -)

### Security for tool-using assistants
- (2022-09-??) **Prompt Injection Attacks Against NLP Systems** [📝 Paper](https://arxiv.org/abs/2209.07753)  
  *Early framing of injection-style attacks and their implications.*  
  (Type: Paper, Autonomy: -)

- (2023-??-??) **MITRE ATLAS (Adversarial Threat Landscape for AI Systems)** [🌐 Site](https://atlas.mitre.org/)  
  *Threat vocabulary and mapping framework used in practical assistant threat models.*  
  (Type: Resource, Autonomy: -)
