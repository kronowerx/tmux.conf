# tmux.conf

My tmux configuration, using [TPM](https://github.com/tmux-plugins/tpm) for plugins
and the [Catppuccin](https://github.com/catppuccin/tmux) frappé theme.

## Install

```sh
git clone https://github.com/kronowerx/tmux.conf.git ~/.config/tmux
git clone https://github.com/tmux-plugins/tpm ~/.config/tmux/plugins/tpm
tmux source ~/.config/tmux/tmux.conf
```

Then press `prefix + I` inside tmux to install the plugins.

`plugins/` is gitignored — TPM manages its contents.

## Ghostty

Use Ghostty's default `TERM=xterm-ghostty` outside tmux; panes use
`tmux-256color`. The configuration enables true color, hyperlinks, styled
underlines, extended keys, OSC 52 clipboard access, and image passthrough.
It also refreshes `TERM` and `TERM_PROGRAM` when creating or attaching sessions.

After reloading an existing session, detach and reattach from Ghostty, then
open new panes so applications receive the updated environment.
