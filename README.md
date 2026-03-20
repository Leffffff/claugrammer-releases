# Claugrammer

An infinite canvas desktop app for managing multiple Claude Code terminal sessions across projects.

Built with Tauri v2, React, and xterm.js.

![Claugrammer](https://img.shields.io/badge/version-0.3.0-7c3aed) ![Platform](https://img.shields.io/badge/platform-macOS%20%7C%20Windows%20%7C%20Linux-000)

## Install

**macOS (one-line):**

```bash
curl -sL https://github.com/Leffffff/claugrammer-releases/releases/latest/download/install.sh | bash
```

**macOS (manual):** Download `.dmg` from [Releases](https://github.com/Leffffff/claugrammer-releases/releases), drag to Applications. If blocked: `xattr -cr /Applications/Claugrammer.app`

**Windows:** Download `.msi` from [Releases](https://github.com/Leffffff/claugrammer-releases/releases) and run the installer.

**Linux:** Download `.deb` or `.AppImage` from [Releases](https://github.com/Leffffff/claugrammer-releases/releases).

```bash
# Debian/Ubuntu
sudo dpkg -i claugrammer_*.deb

# AppImage
chmod +x Claugrammer_*.AppImage && ./Claugrammer_*.AppImage
```

## What is this?

Claugrammer gives you an infinite canvas where you can create **workspaces** — each workspace bundles:

- **Claude terminal** — runs Claude Code in your project folder
- **Exec terminal** — for running dev commands (npm dev, etc.)
- **Web preview** — iframe showing your dev server with auto port detection
- **Plan view** — todo list synced to `.claugrammer/PLAN.md` (Claude can read it)
- **Diff viewer** — live git diff with syntax highlighting
- **File tree** — browse workspace files, send paths to Claude

All windows live on an infinite canvas you can pan, zoom, and organize freely.

## Features

### Canvas
- Infinite pan and zoom
- 4 canvas themes (Dots, Lines, Blueprint, Clean)
- Minimap navigation
- Sticky notes / annotations
- Workspace frames (visual grouping)
- Auto-layout, focus mode, multiple pages

### Terminals
- Real PTY terminals (portable-pty)
- 6 color themes (Dark, Dracula, Monokai, Nord, Solarized, Light)
- Right-click context menu, status indicators, git branch display
- Drag files from Finder to paste paths

### Workspace Management
- Project templates (Next.js, Vite, Remix, Python, Rails, Electron)
- Auto port detection, terminal linking, workspace collapse
- Close confirmation for active sessions

### Productivity
- Recipes (save and replay command sequences)
- Shared clipboard between terminals
- Session persistence across restarts
- Resource monitor (CPU/memory)
- Screenshot (full window capture)
- Notifications when Claude finishes
- Onboarding flow and settings page

## Auto-updates

The app checks for updates on startup and installs them automatically.

## Requirements

- **macOS** 10.15+
- **Windows** 10+
- **Linux** with WebKitGTK 4.1
- [Claude Code CLI](https://docs.anthropic.com/en/docs/claude-code) installed
