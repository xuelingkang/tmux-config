# tmux-config

Personal tmux configuration.

## Requirements

- tmux 3.3a+ (for `%if` / `%endif` preprocessor and `#{host_os}` format)

## Features

- Mouse support
- macOS IME auto-switch: automatically switches to ABC (English) input method when entering a pane or pressing prefix (`C-b`)
- Alt + hjkl pane navigation
- vi-style copy mode
- [TPM](https://github.com/tmux-plugins/tpm) plugin manager with sensible, copycat, yank, open, and nord theme

## Notes

The IME switching section is guarded by `%if #{==:#{host_os},Darwin}` — non-macOS systems skip it silently.
