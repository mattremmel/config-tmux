# config-tmux

My personal tmux configuration.

## Prerequisites

- `tmux` (3.0+ recommended)
- `git`

## Install

1. Clone this repo:

   ```sh
   git clone <repo-url> ~/workspace/personal/config-tmux
   ```

2. Symlink `.tmux.conf` into your home directory:

   ```sh
   ln -s ~/workspace/personal/config-tmux/.tmux.conf ~/.tmux.conf
   ```

   Or, if you prefer a copy:

   ```sh
   cp ~/workspace/personal/config-tmux/.tmux.conf ~/.tmux.conf
   ```

3. Install [TPM](https://github.com/tmux-plugins/tpm) (Tmux Plugin Manager):

   ```sh
   git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
   ```

4. Start tmux:

   ```sh
   tmux
   ```

5. Install plugins from inside tmux by pressing the prefix followed by `I` (capital i):

   ```
   Ctrl-b   I
   ```

   TPM will fetch and install all plugins listed in `.tmux.conf`. The status bar should update with the Catppuccin theme once done.

## Reloading after changes

After editing `~/.tmux.conf`, reload it from inside tmux:

```
Ctrl-b   r
```

## Plugins included

- [tpm](https://github.com/tmux-plugins/tpm) — plugin manager
- [tmux-sensible](https://github.com/tmux-plugins/tmux-sensible) — sane defaults
- [vim-tmux-navigator](https://github.com/christoomey/vim-tmux-navigator) — seamless pane navigation with vim
- [catppuccin/tmux](https://github.com/catppuccin/tmux) — Catppuccin (mocha) theme
