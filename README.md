<div align="center">

```text
██████╗ ██████╗ ██████╗  ██████╗  ██████╗ ██████╗ 
██╔══██╗╚════██╗██╔══██╗██╔════╝ ██╔═████╗██╔══██╗
██████╔╝ █████╔╝██║  ██║██║  ███╗██║██╔██║██║  ██║
██╔══██╗ ╚═══██╗██║  ██║██║   ██║████╔╝██║██║  ██║
██║  ██║██████╔╝██████╔╝╚██████╔╝╚██████╔╝██████╔╝
╚═╝  ╚═╝╚═════╝ ╚═════╝  ╚═════╝  ╚═════╝ ╚═════╝ 
```

### `user@zionsec:~$ whoami`

**24-year-old software engineer from California.**  
Moving from Linux to Windows 11 to build open-source software for gamers — focused on video games, game development, and software engineering for players.

[![Website](https://img.shields.io/badge/site-r3dg0d.github.io-00ff66?style=for-the-badge&labelColor=0a0a0a)](https://r3dg0d.github.io)
[![GitHub](https://img.shields.io/badge/github-r3dg0d-00ff66?style=for-the-badge&labelColor=0a0a0a&logo=github&logoColor=00ff66)](https://github.com/r3dg0d)
[![Windows 11](https://img.shields.io/badge/now_on-Windows_11-0078D4?style=for-the-badge&labelColor=0a0a0a&logoColor=white)](https://www.microsoft.com/windows/windows-11)
[![Focus](https://img.shields.io/badge/focus-open_source_for_gamers-00ff66?style=for-the-badge&labelColor=0a0a0a)](#now-playing)

</div>

---

## About

I'm a software engineer based in California, and I'm changing direction: I'm **moving away from Linux (NixOS) to Windows 11** and pointing my work at games.

- 🎮 **Open-source software for gamers** — tools, mods, and utilities built for players first
- 🕹️ **More video games and game development**
- 🛠️ **Software engineering for players** — the same small, focused repos and honest docs as before

My earlier public work is practical Linux tooling: privacy/OPSEC CLIs, Hyprland desktop utilities, and local AI pipelines. Those repos stay up and documented below.

---

## Now playing

Gaming projects already on my GitHub:

| Repo | What it does |
|------|----------------|
| [`stream-able`](https://github.com/r3dg0d/stream-able) | OBS-like recording/livestream studio inside Minecraft |
| [`vanillaamericamc`](https://github.com/r3dg0d/vanillaamericamc) | Vanilla America+ MC server, portal, plugins, NixOS deploy |
| [`nixpresence`](https://github.com/r3dg0d/nixpresence) | VRChat OSC chatbox and optional Discord presence with modular Linux data sources |

---

## Workstation — `zionsec`

| | |
|---|---|
| **Host** | MAINGEAR MG-1 · moving to Windows 11 (previously NixOS 26.11) |
| **CPU** | Intel Core i9-14900K · 24 cores / 32 threads |
| **GPU** | NVIDIA GeForce RTX 4090 · 24 GB VRAM |
| **RAM** | 31 GiB (no swap) |
| **Storage** | ~1.8 TB NVMe (T-FORCE) + ~1 TB secondary |
| **Desktop** | Windows 11 (was Hyprland · Ghostty · PipeWire) |

Last NixOS snapshot, before the switch:

```bash
$ neofetch --stdout | head
neo@zionsec
-----------
OS: NixOS 26.11.19800101.dirty (Zokor) x86_64
Host: MAINGEAR MG-1
Kernel: 7.2.5
CPU: Intel i9-14900K (32) @ 6.0GHz
GPU: NVIDIA GeForce RTX 4090
Memory: 31GiB
```

---

## Earlier work — Linux / NixOS

### PRIV / SEC toolkit
Honest Linux OPSEC CLIs — independent repos + umbrella.

| Repo | What it does |
|------|----------------|
| [`privsec-tools`](https://github.com/r3dg0d/privsec-tools) | Umbrella directory + Nix package set |
| [`macrandom`](https://github.com/r3dg0d/macrandom) | MAC randomizer with NetworkManager awareness |
| [`mullvadctl`](https://github.com/r3dg0d/mullvadctl) | Mullvad companion — status, relays, privacy session |
| [`dnscheck`](https://github.com/r3dg0d/dnscheck) | DNS privacy analyzer (resolv / resolved / NM / Mullvad) |
| [`netidentity`](https://github.com/r3dg0d/netidentity) | Local network identity snapshot + diff |
| [`metaclean`](https://github.com/r3dg0d/metaclean) | Metadata inspector / scrubber (EXIF, GPS, Office, media) |
| [`fileshred`](https://github.com/r3dg0d/fileshred) | Secure-delete CLI that explains SSD/CoW/TRIM limits |
| [`browserprivacy`](https://github.com/r3dg0d/browserprivacy) | Read-only Chromium/Firefox privacy audit |
| [`opsec-check`](https://github.com/r3dg0d/opsec-check) | Umbrella privacy/security audit CLI |
| [`fakeperson`](https://github.com/r3dg0d/fakeperson) | Photorealistic fictional people + persistent IDs |
| [`aivoice`](https://github.com/r3dg0d/aivoice) | Local real-time AI voice conversion (PipeWire mic) |
| [`deepfake`](https://github.com/r3dg0d/deepfake) | Face-swap CLI for research/VFX (AlphaFace) |

### Desktop / Linux
| Repo | What it does |
|------|----------------|
| [`Nala-Voice`](https://github.com/r3dg0d/Nala-Voice) | Hyprland companion fork with a local voice assistant (experimental) |
| [`dotfiles`](https://github.com/r3dg0d/dotfiles) | Audited NixOS workstation — Hyprland, Ambxst, Ghostty |
| [`matrix`](https://github.com/r3dg0d/matrix) | Realtime Matrix-style digital rain for the terminal (Rust) |
| [`MatrixShot`](https://github.com/r3dg0d/MatrixShot) | Wayland screenshot + screen recording suite |
| [`vmtools`](https://github.com/r3dg0d/vmtools) | windowsvm / linuxvm / androidvm — NixOS-friendly VM CLIs |
| [`ai-media-cli`](https://github.com/r3dg0d/ai-media-cli) | Local-first AI media CLI (Qwen text2img/img2img, 3dai, editvideo) |
| [`KeystrokeNoise`](https://github.com/r3dg0d/KeystrokeNoise) | Multi-keyboard mechanical clicks + mouse sounds (evdev) |
| [`matrix-code-rain-sddm`](https://github.com/r3dg0d/matrix-code-rain-sddm) | Matrix Katakana SDDM greeter theme |

### Other
| Repo | What it does |
|------|----------------|
| [`r3dg0d.github.io`](https://github.com/r3dg0d/r3dg0d.github.io) | Personal site → [r3dg0d.github.io](https://r3dg0d.github.io) |

---

## Stack

<p align="center">
  <img src="https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white" alt="Rust" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Nix-5277C3?style=for-the-badge&logo=nixos&logoColor=white" alt="Nix" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Windows_11-0078D4?style=for-the-badge&logoColor=white" alt="Windows 11" />
  <img src="https://img.shields.io/badge/Java_(Minecraft)-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java (Minecraft)" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" alt="Linux" />
  <img src="https://img.shields.io/badge/CUDA-76B900?style=for-the-badge&logo=nvidia&logoColor=white" alt="CUDA" />
  <img src="https://img.shields.io/badge/Hyprland-58E1FF?style=for-the-badge&logoColor=black" alt="Hyprland" />
  <img src="https://img.shields.io/badge/Wayland-FF5555?style=for-the-badge&logo=wayland&logoColor=white" alt="Wayland" />
</p>

<p align="center"><sub>Learning / exploring for game dev:</sub><br/>
  <img src="https://img.shields.io/badge/C%23-512BD4?style=flat-square&logoColor=white" alt="C#" />
  <img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white" alt="C++" />
  <img src="https://img.shields.io/badge/Unity-000000?style=flat-square&logo=unity&logoColor=white" alt="Unity" />
  <img src="https://img.shields.io/badge/Unreal_Engine-0E1128?style=flat-square&logo=unrealengine&logoColor=white" alt="Unreal Engine" />
  <img src="https://img.shields.io/badge/Godot-478CBF?style=flat-square&logo=godotengine&logoColor=white" alt="Godot" />
</p>

---

## GitHub

<div align="center">

<img height="180" src="https://github-readme-stats.anuraghazra1.vercel.app/api?username=r3dg0d&show_icons=true&hide_border=true&bg_color=0a0a0a&title_color=00ff66&icon_color=00ff66&text_color=eaeaea&ring_color=00ff66" alt="r3dg0d GitHub stats" />
<img height="180" src="https://github-readme-stats.anuraghazra1.vercel.app/api/top-langs/?username=r3dg0d&layout=compact&hide_border=true&bg_color=0a0a0a&title_color=00ff66&text_color=eaeaea" alt="Top languages" />

<br/>

[![GitHub Streak](https://streak-stats.demolab.com?user=r3dg0d&theme=chartreuse-dark&hide_border=true&background=0A0A0A&ring=00FF66&fire=00FF66&currStreakLabel=00FF66)](https://git.io/streak-stats)

</div>

---

<div align="center">

```text
┌─────────────────────────────────────────────┐
│  building for players · california · win11 │
│  https://r3dg0d.github.io                   │
└─────────────────────────────────────────────┘
```

<sub>Profile README · special repo <code>r3dg0d/r3dg0d</code> · now on Windows 11</sub>

</div>
