# tmux-config

A professional, modern `tmux` configuration featuring the **Ayu Dark** theme, session persistence, and Vim-style navigation. Optimized for performance, aesthetics, and portability.

## ✨ Features

- **🎨 Theme:** Ayu Dark variant (via `Saecki/tmux-ayu`) with a clean, centered status bar.
- **💾 Persistence:** Automatic session saving every 15 minutes and manual restore (via `tmux-resurrect` & `tmux-continuum`).
- **⌨️ Navigation:** Seamless Vim-style pane navigation and resizing.
- **🚀 Portability:** Automatic installation of TPM (Tmux Plugin Manager) on first run.
- **🖼️ Modern Support:** True Color (24-bit RGB) and image passthrough (for Yazi/Neovim) enabled.
- **📂 XDG Compliant:** Located in `~/.config/tmux/`.

## 🚀 Installation

To install this configuration on a fresh machine, run:

```bash
# 1. Create the config directory
mkdir -p ~/.config

# 2. Clone this repository
git clone https://github.com/landxcape/tmux-config ~/.config/tmux

# 3. Start tmux
tmux
```

*Note: TPM and all plugins will automatically install on the first run thanks to the bootstrap script in `tmux.conf`.*

## ⌨️ Keybindings

The prefix key is **`Ctrl-b`**.

### General
- `prefix + r` - Reload configuration.
- `prefix + c` - New window in current path.
- `prefix + |` - Split pane horizontally.
- `prefix + -` - Split pane vertically.
- `prefix + L` - Toggle between last two windows.
- `prefix + z` - Zoom/Unzoom current pane.

### Pane Navigation (Vim-style)
- `Alt + h/j/k/l` - Direct pane switching (no prefix needed, works with `vim-tmux-navigator`).

### Pane Resizing
- `prefix + H` - Resize left (5 cells).
- `prefix + J` - Resize down (5 cells).
- `prefix + K` - Resize up (5 cells).
- `prefix + L` - Resize right (5 cells).

### Session Persistence
- `prefix + Ctrl-s` - Manual save.
- `prefix + Ctrl-r` - Manual restore.

## 🛠️ Requirements
- **tmux** 3.2+ (for full feature support).
- A terminal with **True Color** support (e.g., Alacritty, Kitty, WezTerm, iTerm2).
- A Nerd Font for icon support (optional but recommended).

---
*Created by [landxcape](https://github.com/landxcape)*
