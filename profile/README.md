<h1 align="center">Pulsar</h1>

<p align="center">
  Free, open-source <b>remote desktop and game streaming</b>. An alternative to TeamViewer, AnyDesk, Parsec and
  RustDesk, with no account and no telemetry.
</p>

<p align="center">
  <a href="https://pulsardesk.com"><img src="https://img.shields.io/badge/website-pulsardesk.com-5B57E0?style=for-the-badge" alt="Website"></a>
  <img src="https://img.shields.io/badge/status-alpha-orange?style=for-the-badge" alt="Status">
  <img src="https://img.shields.io/badge/license-GPL--3.0-5B57E0?style=for-the-badge" alt="License">
</p>

---

## What is Pulsar?
Pulsar does two things with one app:

- **Remote desktop:** reach your own computer from anywhere, or help a friend with theirs.
- **Game streaming:** play games running on another PC with a controller, keyboard or mouse.

To connect, enter the other device's **ID and one-time password**. Pulsar connects the two devices directly when the
network allows it, and through a relay server when it doesn't. Every session is end-to-end encrypted, so the relay
only forwards data it cannot read. The relay is open source too, and you can run your own.

---

## Highlights
- **Game streaming:** up to 4K and 240 fps, H.264 / H.265 / AV1, 10-bit HDR, a stream that keeps tuning itself to
  the link, FSR / NVIDIA RTX / Intel video upscaling, and a real DualSense on the host (adaptive triggers, haptics,
  headset jack, mic).
- **Remote desktop:** browser-like tabs you can tear off and merge, split screen, multi-monitor, file manager,
  clipboard, chat and microphone.
- **Security:** end-to-end encryption that is always on (PAKE with forward secrecy), approve / deny, trusted
  devices, unattended access and two-factor authentication.
- **Network:** peer-to-peer first (NAT punching, UPnP / NAT-PMP, works over ZeroTier and Tailscale), with a relay you
  can host yourself.

---

## Projects
| Project | What it does | Platforms |
|---|---|---|
| [**Pulsar Desktop**](https://github.com/PulsarDesk/pulsar-desktop) | The app for computers | Windows, macOS, Linux (x64, arm64) |
| [**Pulsar Mobile**](https://github.com/PulsarDesk/pulsar-mobile) | The app for phones and tablets | Android, iOS (not released yet) |
| [**Relay**](https://github.com/PulsarDesk/relay) | Your own Pulsar server | Docker, Linux, Windows, macOS |
| [**Website**](https://github.com/PulsarDesk/web) | [pulsardesk.com](https://pulsardesk.com) | — |

Shared building blocks: [pulsar-core](https://github.com/PulsarDesk/pulsar-core) (the streaming engine both apps use),
[pulsar-proto](https://github.com/PulsarDesk/pulsar-proto) (the network protocol) and
[design](https://github.com/PulsarDesk/design) (colors, fonts, screens).

Everything is in early (alpha) development. Each app's README lists the systems and graphics cards it has been tested
on.

---

## Download
- **Computer:** [pulsar-desktop releases](https://github.com/PulsarDesk/pulsar-desktop/releases/latest)
- **Android:** [Pulsar-android.apk](https://github.com/PulsarDesk/pulsar-mobile/releases/latest/download/Pulsar-android.apk)
- Or visit [pulsardesk.com](https://pulsardesk.com), which picks the right file for your system.

---

## Found a bug?
Open an issue in the repository of the app you were using:
[desktop](https://github.com/PulsarDesk/pulsar-desktop/issues/new/choose) or
[mobile](https://github.com/PulsarDesk/pulsar-mobile/issues/new/choose). Reports from real devices help the most.
Include your operating system, graphics card and the app's log file.

---

## Contributing
Issues and pull requests are welcome in every project repository.

---

## License
All Pulsar projects are licensed under **GNU GPLv3 or later** (GPL-3.0-or-later).
