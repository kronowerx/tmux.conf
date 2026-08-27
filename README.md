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
