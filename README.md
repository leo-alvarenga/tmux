# Tmux

A maintainable, ready-to-use _[tmux](https://github.com/tmux/tmux)_ config that separates core behavior from styling using sourced `.conf` files simple to extend, easy to style.

> Make sure to also check my Neovim configuration, which is designed to work seamlessly with this Tmux setup: [leo-alvarenga/nvim](https://github.com/leo-alvarenga/nvim)

## Setup

```bash
git clone https://github.com/leo-alvarenga/tmux "$HOME/.config/tmux"
```

## Previews (using the Kanagawa theme)

#### Classic layout

Default:
[!Classic default](./docs/classic.png)

Mono:
[!Classic mono](./docs/classic-mono.png)

#### Bubble layout

Default:
[!Bubble default](./docs/bubble.png)

Mono:
[!Bubble mono](./docs/bubble-mono.png)

#### Powerline layout

Default:
[!Powerline default](./docs/powerline.png)

Mono:
[!Powerline mono](./docs/powerline-mono.png)

## Layout

```
tmux.conf                 # orchestrator: sources base → theme → layout
base/                     # behavior (options, keymaps, plugins)
themes/                   # color palettes (swap in tmux.conf)
layouts/                  # status-bar looks (swap in tmux.conf)
```

## Theming

Themes define color variables only (palette + generic aliases like `accent`, `bgSurface`, `text`); layouts paint the status bar, borders and message line with those names. Any theme + any layout can be combined.

**Themes** (edit the `source-file` line in `tmux.conf`):

- `themes/kanagawa.conf`: Kanagawa Wave (default)
- `themes/everforest.conf`: Everforest (dark, medium)

To add a theme: copy an existing one and redefine the generic aliases at the bottom of the file; the contracts are documented there.

**Layouts** (edit the `source-file` line in `tmux.conf`):

- `layouts/classic.conf`: classic powerline chevron separators, colorful (default)
- `layouts/classic-mono.conf`: same look, monochromatic
- `layouts/bubble.conf`: rounded pill separators, colorful
- `layouts/bubble-mono.conf`: same look, monochromatic
- `layouts/powerline.conf`: angled slash separators, colorful
- `layouts/powerline-mono.conf`: same look, monochromatic

### Note for tmux >= 3.7

Prompts and messages overlay the status line instead of replacing it. `message-style`/`message-command-style` therefore include `fill=…` so the bar spans the full width; keep `fill` when restyling.

## License

[MIT License](./LICENSE.md)
