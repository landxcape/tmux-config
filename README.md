# tmux-config

A professional, modern `tmux` configuration featuring the **Ayu Dark** theme, session persistence, and Vim-style navigation. Optimized for performance, aesthetics, and portability.

## ✨ Features

- **🎨 Theme:** Ayu Dark variant with a clean, centered status bar and `gitmux` status indicator.
- **💾 Persistence:** Automatic session saving every 15 minutes and manual restore (via `tmux-resurrect` & `tmux-continuum`).
- **⌨️ Navigation:** Seamless Vim-style pane navigation and resizing (`vim-tmux-navigator`).
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
- `prefix + |` - Split pane horizontally (current path).
- `prefix + -` - Split pane vertically (current path).
- `prefix + Tab` - Toggle between last two windows.
- `prefix + o` - Fuzzy-finder popup switcher for sessions/windows (`fzf`).
- `prefix + s` - Session tree viewer.
- `prefix + S` - Toggle pane synchronization.
- `prefix + z` - Zoom/Unzoom current pane.
- `prefix + b` - Break current pane into a background window.
- `prefix + j` - Join pane from another window.
- `prefix + x` - Kill current pane without confirmation.
- `prefix + X` - Kill current window without confirmation.
- `prefix + Q` - Kill session (prompts for confirmation).

### Navigation
- `Ctrl + h/j/k/l` - Direct pane switching (works seamlessly with Neovim via `vim-tmux-navigator`).
- `Alt + Arrow Keys` - Direct pane switching without prefix.
- `Shift + Left/Right` - Switch to previous/next window.

### Pane Resizing
- `prefix + H` - Resize left (5 cells).
- `prefix + J` - Resize down (5 cells).
- `prefix + K` - Resize up (5 cells).
- `prefix + L` - Resize right (5 cells).

### Copy Mode (Vi)
- `prefix + [` - Enter copy mode.
- `v` - Begin selection.
- `y` / `Enter` - Copy selection to system clipboard (`pbcopy`) and cancel.

### Session Persistence
- `prefix + Ctrl-s` - Manual save.
- `prefix + Ctrl-r` - Manual restore.

## 🛠️ Requirements
- **tmux** 3.2+ (for full feature support).
- **fzf** (for `prefix + o` popup switcher).
- **gitmux** (for status bar git information).
- A terminal with **True Color** support (e.g., Alacritty, Kitty, WezTerm, Ghostty, iTerm2).
- A Nerd Font for icon support (optional but recommended).

---
*Created by [landxcape](https://github.com/landxcape)*
