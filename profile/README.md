<p align="center">
  <img width="120" height="120" src="https://raw.githubusercontent.com/PulsarDesk/.github/main/profile/logo.svg" alt="Pulsar Logo">
</p>

<h1 align="center">Pulsar</h1>

<p align="center">
  A <b>free, open-source</b> remote-desktop &amp; game-streaming app — a self-hostable
  alternative to Parsec, TeamViewer, AnyDesk and RustDesk. ⚡
</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-alpha-orange?style=for-the-badge" alt="Status">
  <img src="https://img.shields.io/maintenance/yes/2026?style=for-the-badge" alt="Maintained">
  <img src="https://img.shields.io/badge/license-GPLv3-5B57E0?style=for-the-badge" alt="License">
  <img src="https://img.shields.io/badge/platforms-Windows%20·%20macOS%20·%20Linux%20·%20Android%20·%20iOS-5B57E0?style=for-the-badge" alt="Platforms">
</p>

---

## ⚡ What is Pulsar?

One app, two jobs:

- 🎮 **Game streaming** *(Sunshine/Parsec-style)* — low-latency remote play, controller +
  keyboard/mouse, hardware **H.265 / AV1**, up to **120 fps**, **HDR**.
- 🖥️ **Remote desktop & management** *(TeamViewer/RustDesk-style)* — connect with a
  device **ID + one-time password**, unattended access, file transfer, multi-monitor.

Built for **gamers** (latency first) and **IT / support teams**. Runs on **Windows,
macOS, Linux, Android and iOS**.

---

## 🔒 How it connects

- **Automatic P2P → relay.** Pulsar tries a **direct peer-to-peer** connection first and
  **automatically falls back to a relay** when NAT/firewall hole-punching fails. Never an
  either/or choice.
- **You own the identity.** The **device ID is issued by the relay** — and the relay is
  **self-hostable**, so identity distribution *and* fallback transport can be fully yours.
- **End-to-end encrypted, zero-knowledge.** X25519 + ChaCha20-Poly1305; keys live only on
  your devices; the relay only ever forwards ciphertext. **No account. No telemetry.**

---

## 📢 Release Types

Pulsar is currently in **Alpha** (0.x). Releases are cut automatically from
[Conventional Commits](https://www.conventionalcommits.org/):

- **Alpha** — early-stage. Experimental features, possible breaking changes, rough edges.
- **Beta** — feature-complete and generally stable. Good for early adopters.
- **Release** — stable and production-ready.

---

## 📦 Repositories

| Repo | What |
| ---- | ---- |
| [**pulsar-desktop**](https://github.com/PulsarDesk/pulsar-desktop) | Desktop app — Windows / macOS / Linux (Tauri 2 · SvelteKit · Rust) |
| [**pulsar-mobile**](https://github.com/PulsarDesk/pulsar-mobile) | Mobile app — Android + iOS (Tauri 2) |
| [**pulsar-core**](https://github.com/PulsarDesk/pulsar-core) | Shared engine — client/host/streaming core (Rust); both apps depend on it |
| [**relay**](https://github.com/PulsarDesk/relay) | Self-hostable rendezvous / relay server (Rust, tokio UDP) |
| [**pulsar-proto**](https://github.com/PulsarDesk/pulsar-proto) | Shared wire protocol (relay ↔ apps) |
| [**web**](https://github.com/PulsarDesk/web) | Marketing site (SvelteKit on Cloudflare Pages) |
| [**design**](https://github.com/PulsarDesk/design) | Design system &amp; brand handoff (tokens are the source of truth) |

---

## ⬇️ Trying Pulsar

Grab the latest desktop build from
[**pulsar-desktop/releases**](https://github.com/PulsarDesk/pulsar-desktop/releases) —
Windows, macOS, Linux (x64 **and** ARM64 for Orange Pi / Raspberry Pi) — or the mobile
build from [**pulsar-mobile/releases**](https://github.com/PulsarDesk/pulsar-mobile/releases)
(Android + iOS).

Want your own relay? Download a prebuilt binary from
[**relay/releases**](https://github.com/PulsarDesk/relay/releases), point your devices at
`your-host:port`, and you're self-hosting.

---

## 🛠️ Built with

- **Rust** — the performant client / host / streaming core, the relay, and the shared protocol.
- **Tauri 2 + SvelteKit (Svelte 5)** — one cross-platform shell for both the *client* and *host* roles.
- **gilrs / uinput / ViGEmBus** — controller capture and virtual-gamepad replay.
- Hardware A/V — **NVENC · AMF · QuickSync · VideoToolbox · VAAPI**, software baseline everywhere.

---

## 🤝 Contributing

Issues and pull requests are welcome across all repositories. Each repo runs CI (Rust +
JS tests) on every push and PR; releases are cut by semantic-release from Conventional
Commits. Please keep tests green and follow the existing style.

---

## 📄 License

Every Pulsar repository is licensed under the **GNU General Public License v3.0**
(**GPLv3**) — fully open source. See each repo's `LICENSE` for details.
