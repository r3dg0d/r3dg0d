<div align="center">

```text
██████╗ ██████╗ ██████╗  ██████╗  ██████╗ ██████╗ 
██╔══██╗╚════██╗██╔══██╗██╔════╝ ██╔═████╗██╔══██╗
██████╔╝ █████╔╝██║  ██║██║  ███╗██║██╔██║██║  ██║
██╔══██╗ ╚═══██╗██║  ██║██║   ██║████╔╝██║██║  ██║
██║  ██║██████╔╝██████╔╝╚██████╔╝╚██████╔╝██████╔╝
╚═╝  ╚═╝╚═════╝ ╚═════╝  ╚═════╝  ╚═════╝ ╚═════╝ 
```

**Open-source software for gamers and players** — video games, game development, and the tools around them.

[![Website](https://img.shields.io/badge/site-r3dg0d.github.io-b46bff?style=for-the-badge&labelColor=0a0a0a)](https://r3dg0d.github.io)
[![GitHub](https://img.shields.io/badge/github-r3dg0d-00ff66?style=for-the-badge&labelColor=0a0a0a&logo=github&logoColor=00ff66)](https://github.com/r3dg0d?tab=repositories)

</div>

---

## Projects

### Games & player tools

#### [`stream-able`](https://github.com/r3dg0d/stream-able) · Java

An OBS-like recording, livestreaming and multistreaming studio that runs inside Minecraft as a Fabric mod (MC 26.1.2 / 26.2 / 26.3), successor to Record-able. It adds RTMP/RTMPS streaming and multistreaming, interactive Chromium browser sources composited over gameplay, a microphone chain with optional local AI noise cancellation, and ultrawide support. Everything is driven from an in-game Studio screen (F6), and FFmpeg, the browser engine and models are downloaded on demand, pinned and SHA-256 verified.

#### [`vanillaamericamc`](https://github.com/r3dg0d/vanillaamericamc) · Java

Vanilla America+ is a client-mod-free Paper server project for Java and Bedrock cross-play. The repo holds the custom Paper plugin, a local operations portal, BlueMap integration, audited reports, a mock-only shop and a NixOS deployment module. Deployments default to loopback-only listeners and never accept the EULA, open public ports or enable live payments on their own.

#### [`nixpresence`](https://github.com/r3dg0d/nixpresence) · Rust

A VRChat OSC chatbox compositor with an optional Discord Rich Presence daemon, inspired by the ideas behind MagicChatBox but written independently under MIT. Providers such as MPRIS music and the focused window feed a shared state that is templated and sent to VRChat OSC, Discord or stdout. It includes doctor, preview and test commands and a systemd user service.


### Creative & AI media

#### [`ai-media-cli`](https://github.com/r3dg0d/ai-media-cli) · Python

A local-first AI media CLI suite: Qwen-Image text-to-image and image editing, 3dai for a multi-stage TRELLIS.2 3D asset pipeline, and editvideo for SCAIL-2 character animation jobs. An ai-media doctor command checks environment, GPU and terminal-graphics support. Model weights are never bundled, and the shared preview/config tooling works without a GPU.

#### [`aivoice`](https://github.com/r3dg0d/aivoice) · Python

Local real-time AI voice conversion built on MeanVC2, exposed as a PipeWire virtual microphone. It searches community voice catalogs, downloads and validates voices, and builds reusable zero-shot MeanVC2 profiles from reference audio, including an honest RVC-to-MeanVC2 profile migration that does not pretend to convert weights. Usage requires an explicit consent acknowledgement.

#### [`deepfake`](https://github.com/r3dg0d/deepfake) · Python

A real-time face-swap CLI for research and VFX that wraps the AlphaFace research model. It adds an application shell around it: webcam and video capture, detect-swap-composite, presets and metrics, plus OBS-friendly outputs (preview, file, FFmpeg pipe, GStreamer, v4l2loopback virtual camera). A first-run consent notice and a synthetic-media watermark are on by default.

#### [`fakeperson`](https://github.com/r3dg0d/fakeperson) · Python

A CLI for photorealistic fictional people with persistent synthetic identities (seed plus locked facial and style traits) rendered through a pluggable model backend. Safeguards refuse likely real-person or celebrity prompts and stamp every PNG as synthetic. A deterministic stub backend keeps it testable without a GPU.


### Privacy & security

#### [`blurcam`](https://github.com/r3dg0d/blurcam) · C++

Native C++20 face privacy for Linux: YuNet face detection and optical-flow tracking with local blur, pixelation and glitch effects. It processes files through FFmpeg, previews with SDL, and outputs to a v4l2loopback virtual camera. No accounts, cloud inference, uploads or telemetry, and the docs are explicit that detection is fallible and offer a max-privacy preset and box masks.

#### [`privsec-tools`](https://github.com/r3dg0d/privsec-tools) · Nix

The directory for a Linux-first privacy, security and OPSEC CLI toolkit. Every tool lives in its own independent repo; this umbrella indexes them with install commands and versions and optionally exposes a Nix package set. It states plainly that the tools improve hygiene and awareness but do not make anyone anonymous.

#### [`opsec-check`](https://github.com/r3dg0d/opsec-check) · Rust

An umbrella, read-only privacy/OPSEC audit CLI for Linux covering network identity, VPN, DNS, MAC and more, optionally calling sibling tools (macrandom, mullvadctl, dnscheck, netidentity, metaclean, browserprivacy, fileshred) when installed. Findings are classed as informational, attention recommended or configuration issue, each with why it matters, and there is deliberately no fake privacy score. Output as text, JSON, Markdown or HTML.

#### [`macrandom`](https://github.com/r3dg0d/macrandom) · Rust

A Linux MAC-address randomizer with NetworkManager awareness. It lists interfaces with current and permanent MACs, randomizes fully or vendor-preserving, saves originals so they can be restored, and can set per-connection cloned MACs in NetworkManager. VPN, container, bridge and loopback interfaces are skipped by default, and the README documents what MAC randomization does not protect against.

#### [`mullvadctl`](https://github.com/r3dg0d/mullvadctl) · Rust

A companion CLI for the official Mullvad VPN client: status (relay, exit IP, location, DNS, IPv6, kill-switch hints), connect, relay rotation and relay browsing. check verifies connectivity and runs DNS-leak heuristics, and privacy-session snapshots state, optionally randomizes the MAC, connects, verifies and restores on exit. It never reimplements tunnel security and refuses to run without the official mullvad binary.

#### [`dnscheck`](https://github.com/r3dg0d/dnscheck) · Rust

A DNS privacy analyzer that inspects resolv.conf, systemd-resolved, NetworkManager and Mullvad for likely leaks, fallback resolvers, VPN DNS bypass and split DNS. Passive by default, with optional active probes via dig/nslookup. Reports include JSON output and explicit statements of what cannot be detected.

#### [`netidentity`](https://github.com/r3dg0d/netidentity) · Rust

Captures a snapshot of a machine's network identity: hostname, interfaces, IPs and MACs, gateway, VPN, DNS, listening ports, firewall, Wi-Fi SSID and mDNS/UPnP hints. Snapshots are saved as JSON and can be diffed over time to spot changes. An offline mode skips the public-IP lookup, and secrets in free-form fields are redacted.

#### [`metaclean`](https://github.com/r3dg0d/metaclean) · Rust

A metadata inspector and scrubber for JPEG, PNG, WebP, HEIC, MP4, MOV, MP3, FLAC, WAV, PDF and Office files, surfacing GPS, timestamps, camera, author and software tags. It uses mat2 or exiftool when available and built-in Rust fallbacks otherwise. Originals are never overwritten by default: it writes a cleaned copy, and in-place mode makes a backup first.

#### [`fileshred`](https://github.com/r3dg0d/fileshred) · Rust

An honest secure-delete CLI: multi-pass overwrite and unlink on HDDs with non-CoW filesystems, and refusal without explicit acknowledgement on SSD/NVMe, Btrfs/ZFS, network or unknown storage. inspect reports the filesystem, mount options and rotational flag with advice, and explain spells out the limits of wear-leveling, TRIM, snapshots and backups. It never claims a file is guaranteed gone when the storage stack can't guarantee it.

#### [`browserprivacy`](https://github.com/r3dg0d/browserprivacy) · Rust

A read-only privacy auditor for Chromium-family and Firefox-family browser profiles on Linux, including Flatpak variants. It checks WebRTC, DNS-over-HTTPS, proxy mode, cookie policy, site permissions and extension inventories, and counts storage and service-worker entries. It never reads passwords, tokens, cookie values or credential stores.


### Desktop & terminal

#### [`MatrixShot`](https://github.com/r3dg0d/MatrixShot) · QML

A Wayland-native screenshot and screen-recording suite with a Matrix-themed Quickshell overlay. Select a region, then choose Screenshot or Screen Record; recording runs through gpu-screen-recorder with fps and audio options and an on-screen REC indicator. It includes an annotation editor (pen, highlight, rectangle, arrow, text) and uploads the last capture with host failover, copying the URL to the clipboard.

#### [`KeystrokeNoise`](https://github.com/r3dg0d/KeystrokeNoise) · Rust

Subtle mechanical keyboard and mouse click sounds for Linux, run as an evdev daemon across multiple keyboards. Key presses are mapped only to coarse categories (normal, space, enter, modifier, mouse buttons) and discarded immediately, so nothing about what you type is logged or transmitted. Configurable sound packs, a toggle command and a systemd user unit.

#### [`matrix`](https://github.com/r3dg0d/matrix) · Rust

Realtime Matrix-style digital rain for the terminal, built on crossterm. Truecolor palettes with ANSI-256 fallback, presets, charsets and live controls for speed, density, palette and pause. Original glyph sets, XDG config, shell completions and a Nix flake.

#### [`matrix-code-rain-sddm`](https://github.com/r3dg0d/matrix-code-rain-sddm) · QML

A Matrix-inspired SDDM greeter theme for Qt 6: dense Katakana code rain drawn live in QML behind a black-and-green login panel. No video or pre-rendered background, and it imports only QtQuick. The layout scales proportionally from 1080p to ultrawide and 4K, with username selection, masked password entry and a session picker.

#### [`vmtools`](https://github.com/r3dg0d/vmtools) · Python

A CLI/TUI suite for personal virtual machines: windowsvm and linuxvm on QEMU/KVM/libvirt, and androidvm on Docker-Android-Pro, under a vmtools umbrella. Commands cover doctor checks, VM creation from an ISO, interactive terminal menus and desktop entries. It defaults to the per-user libvirt session so disks stay in the user's data directory.

---

<div align="center"><sub><a href="https://r3dg0d.github.io">r3dg0d.github.io</a> · all projects are open source on <a href="https://github.com/r3dg0d">GitHub</a></sub></div>
