# tmux-config

Personal tmux configuration.

## Installation

```bash
# 1. Clone with submodules
git clone --recursive https://github.com/xuelingkang/tmux-config.git ~/.tmux-config

# 2. Symlink config
ln -sf ~/.tmux-config/tmux.conf ~/.tmux.conf

# 3. Install TPM plugins
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
~/.tmux/plugins/tpm/bin/install_plugins
```

> Already have a `~/.tmux.conf`? Back it up first.

## Requirements

- tmux 3.3a+

## Features

- Mouse support
- Alt + hjkl pane navigation
- vi-style copy mode
- [TPM](https://github.com/tmux-plugins/tpm) plugin manager with sensible, copycat, yank, open, and nord theme

## Notes

The IME switching section is guarded by `if-shell` with `uname -s` (macOS) and
`uname -a` (WSL) — non-matching platforms skip them silently.
