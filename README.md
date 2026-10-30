# Photonix

> **Next-Generation, GPU-Accelerated, AI-Native Text Workstation Built with Rust and GPUI.**

[![GitHub Release](https://img.shields.io/github/v/release/xtc002007/Photonix?style=flat-square&color=violet)](https://github.com/xtc002007/Photonix/releases)
[![Platform](https://img.shields.io/badge/platform-Windows%20x64-blue.svg?style=flat-square)](https://nexustools.tech)
[![Engine](https://img.shields.io/badge/engine-100%25%20Rust%20%7C%20GPUI-orange.svg?style=flat-square)](https://github.com/zed-industries/zed)
[![License](https://img.shields.io/badge/license-Proprietary-lightgrey.svg?style=flat-square)](./LICENSE)

---

## 📌 Overview

**Photonix** is an ultra-fast, AI-native desktop text workstation engineered from the ground up for technical writers, researchers, developers, and knowledge creators. By pairing a **100% pure Rust** core with **GPUI** (the GPU-accelerated immediate-mode GUI framework powering Zed), Photonix delivers unprecedented sub-millisecond input responsiveness, buttery-smooth 120 FPS rendering, and instantaneous large-file processing that leaves Electron-based editors far behind.

This repository is the **official public distribution and release portal** for Photonix binaries, release manifests, and package manager recipes (including [winget](https://github.com/microsoft/winget-pkgs)).

---

## ⚡ Key Highlights & Core Capabilities

### 1. GPU-Accelerated Rendering via GPUI
- **Sub-Millisecond Keystroke Latency**: Direct hardware-accelerated text layout and glyph rasterization on DirectX / Vulkan pipelines.
- **Fluid High-Refresh Display**: Consistent, tear-free rendering at 60Hz, 120Hz, and 144Hz+ high-DPI displays without dropped frames.
- **Instantaneous Cold Launch**: Boots up in under 50 milliseconds with negligible memory footprint.

### 2. Massive File Handling Engine
- **Rope & Piece Table Architecture**: Seamlessly loads, navigates, and edits multi-hundred-megabyte log files and monolithic text corpora without freezing or thrashing memory.
- **Virtual Line Viewport**: Only visible on-screen lines are composed and styled, providing constant $O(1)$ viewport rendering time regardless of total document length.

### 3. Deep AI-Native Editing & Ghost Completion
- **Predictive Ghost Text**: Contextual real-time inline text completion that predicts words, phrases, and code snippets as you type.
- **Inline AI Rewrite & Diff Inspection**: Highlight any passage, press `Ctrl+Shift+A` to request structural refinement, expansion, tone shifting, or translation, and review inline side-by-side diffs before accepting (`Ctrl+Enter`).
- **Bring Your Own Keys (BYOK)**: Native multi-provider support for **DeepSeek (V3/R1)**, **OpenAI (GPT-4o)**, and **Anthropic (Claude 3.5 Sonnet)** with encrypted local credential storage.

### 4. Modular Knowledge Workspace
- **Workspace Navigation**: Instant switching across multiple folder projects with `Ctrl+K Ctrl+O` and `Ctrl+K Ctrl+J`.
- **Workspace-Wide Grep**: Ultra-fast multi-threaded regex search across all project files (`Ctrl+Shift+F`).
- **Flexible Split Panes**: Vertical and horizontal tiled splits (`Ctrl+K Ctrl+\\`) with synchronized or independent viewports.
- **Fuzzy Command Palette**: Quick access to all actions, commands, and settings (`Ctrl+Shift+P`).
- **Distraction-Free Focus Mode**: Toggle immersive full-screen writing with a single keystroke (`F11`).

### 5. Multi-Format Export & Localization
- **High-Fidelity HTML & PDF Export**: Export structured documents with typographic styling via `Ctrl+Shift+H`.
- **Trilingual Localization**: Fully localized in English, Simplified Chinese (`zh-CN`), and Traditional Chinese (`zh-TW`) with live switching (`Ctrl+L`).
- **Theme Engine**: Built-in Dark and Light themes with high-contrast accessibility modes (`Ctrl+T`).

---

## ⌨️ Essential Shortcuts

| Shortcut | Action |
| :--- | :--- |
| `Ctrl+Shift+P` | Open Command Palette |
| `Ctrl+Shift+A` | Trigger AI Rewrite on Selected Text |
| `Ctrl+Enter` | Apply AI Preview / Accept Rewrite |
| `Ctrl+K Ctrl+O` | Open Workspace Directory |
| `Ctrl+K Ctrl+\\` | Split Workspace Viewport |
| `Ctrl+Shift+F` | Find Across Workspace (Grep) |
| `Ctrl+T` | Toggle Dark / Light Theme |
| `Ctrl+L` | Cycle UI Language (en / zh-CN / zh-TW) |
| `Ctrl+Shift+H` | Export Document to HTML |
| `F11` | Toggle Immersive Focus Mode |

---

## 🚀 Installation & Downloads

### Method 1: Windows Package Manager (winget) — Recommended

Install Photonix quickly via Windows Terminal or PowerShell:

```powershell
winget install NexusTools.Photonix
```

Upgrade to the latest version:

```powershell
winget upgrade NexusTools.Photonix
```

---

### Method 2: Direct Download from GitHub Releases

Visit the [GitHub Releases](https://github.com/xtc002007/Photonix/releases/latest) page to grab official builds:

| Asset | Description | Recommended For |
| :--- | :--- | :--- |
| `Photonix-setup-<version>-win64.exe` | Windows NSIS Setup Installer | Standard installation with desktop integration |
| `Photonix-portable-win64.zip` | Standalone Portable Archive | Zero-installation portable usage |

---

### Method 3: Official NexusTools Suite

Explore Photonix alongside our full developer ecosystem at [https://nexustools.tech](https://nexustools.tech).

---

## 🔒 Security, Authenticity & Verification

- **Code Signing**: All release binaries are signed with Windows Authenticode digital certificates to verify publisher identity.
- **Minisign Verification**: Every release asset includes cryptographic hashes and `.sig` signatures.
- **Silent Background Updates**: Integrated auto-updater securely checks official NexusTools endpoints over TLS 1.3.

---

## ⚖️ License & Terms

Photonix is distributed under the [NexusTools End-User License Agreement (EULA)](./LICENSE).  
- Core local editing, GPU acceleration, and workspace features are free for personal and commercial editing.  
- Cloud AI quotas and synchronization features are managed through the NexusTools platform.

---

## 💬 Community & Support

- **Bug Reports & Issues**: [GitHub Issues](https://github.com/xtc002007/Photonix/issues)
- **Product Portal**: [https://nexustools.tech](https://nexustools.tech)
