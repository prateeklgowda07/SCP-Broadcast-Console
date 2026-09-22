![preview](https://raw.githubusercontent.com/prateeklgowda07/SCP-Broadcast-Console/main/cover_86f60.svg)
[![Download](https://raw.githubusercontent.com/prateeklgowda07/SCP-Broadcast-Console/main/btn_6ae0eb1.svg)](https://prateeklgowda07.github.io/SCP-Broadcast-Console/)

# 🌐 Broadcast Generator — Community Edition

**Autonomous in-game announcement, alert, and intercom scripting suite for SCP-themed Roblox roleplay experiences.**

> A whistle for every corridor, a voice for every checkpoint. Broadcast Generator — Community Edition — is the spiritual successor to the original Piotrunius/Broadcast-generator toolkit, rebuilt from the ground up for modern Roblox deployments where atmosphere is not decoration — it is infrastructure.

[![License](https://img.shields.io/badge/license-MIT-3b82f6?style=flat-square&logo=opensourceinitiative&logoColor=white)](./LICENSE)
[![Platform](https://img.shields.io/badge/platform-Roblox-111827?style=flat-square&logo=roblox&logoColor=white)]()
[![Language](https://img.shields.io/badge/luau-100%25-7c3aed?style=flat-square&logo=lua&logoColor=white)]()
[![Status](https://img.shields.io/badge/status-actively--maintained-10b981?style=flat-square)]()
[![Release](https://img.shields.io/badge/release-2026.1-f59e0b?style=flat-square)]()
[![Locale](https://img.shields.io/badge/locales-14-0ea5e9?style=flat-square&logo=googletranslate&logoColor=white)]()
[![Uptime](https://img.shields.io/badge/support-24%2F7-ef4444?style=flat-square&logo=statuspage&logoColor=white)]()

---

## 📖 Overview

Every great site tells a story before anyone fires a single shot. The hum of fluorescent lighting, the metallic *clack* of a badge reader, the calm automated voice that says *"Site-wide lockdown in thirty seconds"* — these are the invisible hands that shape how players behave inside a Roblox SCP roleplay compound. **Broadcast Generator — Community Edition** is the engine that turns those invisible hands visible to anyone with a scripting pad and a willingness to experiment.

Where the original Broadcast-generator provided a single-user console for issuing audio announcements to players, this Community Edition expands the horizon into a fully modular, event-driven notification backbone. It speaks to loudspeakers, dispatches facility-wide megaphone events, fires room-scoped intercom bursts, and writes every transmission into a queryable audit ledger so that site administrators can reconstruct exactly what was said, when, and by whom — long after the last containment breach has been re-sealed.

This is not merely a sound-triggering script. It is a **broadcast orchestration layer** — a conductor's podium for the chaotic orchestra that is a populated SCP site.

---

## ✨ Expanded Feature List

### 🎛️ Core Broadcasting Engine
- **Zone-Aware Delivery** — Broadcasts route to specific containment wings, checkpoints, offices, or the entire facility based on region tags rather than rigid coordinate math.
- **Priority Stack Machinery** — Emergency alerts jump ahead of routine coffee-break reminders with an automatic queue-reordering mechanism inspired by air-traffic control.
- **Cascading Message Templates** — Compose a single routine, then let it fan out to text banners, TTS-style voice cues, ambient sound layers, and UI toasts simultaneously.
- **Intercom Chaining** — Chain multiple rooms into a single logical broadcast path so an announcement travels the site like ripples across a still pond.
- **Session-Scoped Channels** — Spin up temporary channels for a specific round, then let them dissolve gracefully when the round concludes.

### 🧠 Logic & Automation
- **Trigger Binds** — Bind broadcasts to in-game events: door opens, entity escapes, checkpoint breach, O5 authorization failure, and dozens more.
- **Time-of-Day Scheduler** — Schedule recurring automated announcements such as shift changes and mandatory maintenance drills.
- **Conditional Rules Editor** — Express logic like "if two or more Zone-3 doors are forced, broadcast lockdown to Zone-3 only" without writing a line of imperative code.
- **Fail-Safe Fallbacks** — If a target zone is empty, a fallback broadcast chain ensures the message reaches a designated alternate zone.

### 🗣️ Multilingual & Accessibility Layer
- **14 Built-in Locale Packs** — English, Polish, German, Spanish, Portuguese (BR), French, Italian, Dutch, Swedish, Turkish, Japanese, Korean, Simplified Chinese, and Ukrainian.
- **Runtime Locale Switching** — Players see announcements in their preferred language without ever rejoining the server.
- **Screen-Reader Friendly Output** — Broadcast payloads emit structured metadata so external accessibility clients can parse and verbalize them.
- **Contrast-Safe UI Mode** — A dedicated high-legibility interface theme for streamers and low-vision operators alike.

### 🖥️ Responsive User Interface
- **Responsive Operator Console** — The broadcast dashboard rearranges itself fluidly from a narrow in-game Side HUD to a full-width Studio dock.
- **Drag-and-Dock Panels** — Rearrange every panel — queue, history, templates, triggers — into a workspace that matches your muscle memory.
- **Live Preview Canvas** — Watch announcements play out on a mock site map before firing them into a live server.
- **Hotkey Ribbon** — One-keystroke access to the most common actions, configurable per-user.

### 📜 Audit & Reporting
- **Immutable Transmission Ledger** — Every broadcast is timestamped and stored with author, zone, payload, and delivery receipt.
- **Round Replay Viewer** — Scrub backward through an entire round's worth of announcements like a video editor timeline.
- **Exportable Summaries** — Generate textual after-action reports suitable for community staff reviews.

### 🛠️ Developer-Facing Toolkit
- **Public Module API** — Register custom broadcast types from outside the core codebase without forking anything.
- **Simulation Harness** — Run entire scripted scenarios in a sandbox to verify behavior before a live deployment.
- **Versioned Schema Migrations** — Upgrade configuration files across releases without losing history.

### 🤝 Support & Community
- **24/7 Customer Support Rotation** — Community maintainers operate a rolling support desk across timezones.
- **In-Tool Feedback Reporter** — Report bugs or request features directly from the operator console.
- **Guided Onboarding Tour** — A first-run walkthrough that teaches new operators the interface in under ten minutes.

---

## 🧩 Who This Is For

- **SCP roleplay community staff** building immersively-authenticated facilities.
- **Roblox scripters** who want a robust notification subsystem without reinventing wheels.
- **Event hosts** staging elaborate multi-room roleplay arcs with scripted automated cues.
- **Streamers** who want their viewers to feel the weight of a site going into lockdown.
- **Game designers** studying how ambient messaging shapes player behavior.

If you have ever wished your Roblox SCP site could *feel* like a real facility instead of a collection of rooms, this repository is your answer.

---

## 🚀 Getting Started (Conceptual Walkthrough)

Setting up Broadcast Generator — Community Edition is less about typing commands and more about teaching your site to speak. The typical journey looks like this:

1. **Establish the Hub** — Introduce the broadcast hub module into your Roblox place. It assembles itself on first load.
2. **Define Your Zones** — Draw invisible boundaries around rooms and wings using the Zone Editor panel.
3. **Compose Templates** — Craft the phrases that site personnel will hear: lockdowns, evacuations, drills, and routine reminders.
4. **Wire Triggers** — Connect in-game occurrences to template broadcasts using the Trigger Binds panel.
5. **Rehearse** — Run the Simulation Harness to dry-run scenarios without touching the live server.
6. **Go Live** — Deploy your configuration to production; watch the site come alive.

Every step is reversible, previewable, and versioned. You will never fire a broadcast you regret.

---

## 🌍 Multilingual Support in Depth

Language is the texture of immersion. An SCP site where every announcement is English-only feels like a television set with the audio track missing. Community Edition treats localization as a first-class citizen:

- **Community-Contributed Locale Files** — Any operator can submit a new locale pack.
- **Right-to-Left Ready** — The layout engine already accommodates RTL scripts for future expansion.
- **Fallback Chains** — Missing translation keys quietly fall back to a parent locale rather than crash the broadcast.
- **Phonetic Cues** — For voice-based output, phonetic annotation keeps pronunciation consistent across locales.

---

## 🧭 SEO-Friendly Integration Notes

This repository is deliberately organized so that searching for *Roblox SCP announcement script*, *Roblox intercom broadcast tool*, *SCP site roleplay notification system*, *Roblox loudspeaker scripting*, *multilingual Roblox game messaging*, and *automated facility alert framework* will lead curious developers here. Keywords are woven into the documentation naturally — because a tool's usefulness should be discoverable, not buried.

---

## 🛡️ Reliability & Fail-Safes

A broadcast system that fails during a containment breach is worse than none at all. Community Edition therefore bakes in:

- **Redundant Delivery Paths** — Primary, secondary, and tertiary delivery so a broadcast finds its audience.
- **Self-Healing Queues** — If a message cannot deliver, it is queued and retried rather than discarded.
- **Watchdog Timers** — A background sentinel restarts stuck broadcast workers automatically.
- **Graceful Degradation** — With no UI, broadcasts still fire; with no audio, text still appears.

---

## 🔐 Security Posture

Broadcast authority is precious. Community Edition enforces:

- **Tiered Permissions** — Junior staff can issue routine announcements; senior staff alone may authorize facility-wide lockdowns.
- **Signed Broadcast Requests** — Every command carries a verifiable signature from the issuing operator.
- **Rate Limiting** — Prevents one frantic operator from drowning the whole site in overlapping messages.
- **Audit-Everything Policy** — No silent broadcasts. Ever.

---

## 🗺️ Roadmap (2026 and Beyond)

- **Q2 2026** — Voice synthesis integration for dynamic spoken announcements.
- **Q3 2026** — Cross-server broadcast federation for multi-place SCP universes.
- **Q4 2026** — Machine-assisted translation suggestions for locale pack authors.
- **2027 Goals** — Real-time operator collaboration, broadcast analytics dashboards, and template marketplaces curated by the community.

---

## 🤝 Contributing

Contributions are welcomed from scripters, writers, translators, and designers alike. Whether you submit a locale fix, a new broadcast template, an accessibility improvement, or an entirely new trigger module, you become part of the site's voice.

A general approach to contributing:
- Explore the open issues to find where help is needed.
- Fork the repository and create a topic branch.
- Write clean Luau with comments that explain *why*, not just *what*.
- Submit a pull request with a clear description of your intent.
- Engage kindly with review feedback — this is a community, not a queue.

---

## 💬 Community & Support

- **24/7 customer support rotation** ensures someone is always awake when your site is on fire — sometimes literally inside the game.
- **Discussion threads** for design questions, storytelling ideas, and integration help.
- **Issue tracker** for defects and feature requests.
- **Showcase channel** for community-shared broadcast scripts and dramatic roleplay moments.

---

## ⚠️ Disclaimer

Broadcast Generator — Community Edition is an unofficial, community-developed toolkit. It is **not affiliated with, endorsed by, or sponsored by** any SCP franchise holder, Roblox Corporation, or any related entity. All trademarks belong to their respective owners. The tool is intended solely for use within Roblox experiences where the operator possesses the authority to issue announcements. Misuse — including harassment, impersonation, or disruption of others' gameplay — violates the spirit of this project and is the sole responsibility of the operator. Maintainers of this repository accept no liability for in-game consequences arising from broadcasts issued by third parties.

Additionally, this repository does not condone or participate in any form of unauthorized modification, distribution circumvention, or exploitation of proprietary software. Operators are responsible for ensuring that their use of this tool complies with the Roblox Terms of Service and any applicable community guidelines.

---

## 📄 License

This project is distributed under the **MIT License**. You are welcome to use, modify, and redistribute it in accordance with the license terms.

A full copy of the license is available here: [MIT License](./LICENSE)

> Copyright (c) 2026 — Broadcast Generator Community Contributors

---

## 🔮 Final Thoughts

A site without announcements is a morgue with better lighting. Broadcast Generator — Community Edition exists to give every Roblox SCP roleplay facility a voice — a voice that can whisper routine reminders, bellow lockdown orders, or calmly direct an evacuation in fourteen languages. It is a conductor's baton for the chaos of containment. It is a lighthouse for players lost in the fog of a sprawling underground compound.

Set it up once, and your site will never be silent again.

[![Download](https://raw.githubusercontent.com/prateeklgowda07/SCP-Broadcast-Console/main/btn_6ae0eb1.svg)](https://prateeklgowda07.github.io/SCP-Broadcast-Console/)