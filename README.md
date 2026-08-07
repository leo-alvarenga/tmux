# Tmux

A maintainable, **dependency-free** _[tmux](https://github.com/tmux/tmux)_ config that separates core behavior from styling using sourced `.conf` files simple to extend, easy to style.

> Make sure to also check my Neovim configuration, which is designed to work seamlessly with this Tmux setup: [leo-alvarenga/nvim](https://github.com/leo-alvarenga/nvim)

## Setup

To setup and use this configuration run this command:

```bash
git clone https://github.com/leo-alvarenga/tmux "$HOME/.config/tmux"
```

## Theming

For now, at least, there is only one theme available `Kanagawa Wave`.

### Style variants

The status bar comes in two interchangeable looks, picked in `tmux.conf`:

- `styles-powerline.conf` — angled slash separators (`\ue0be` / `\ue0ba`) *(default)*
- `styles-bubble.conf` — rounded pill separators (`\ue0b6` / `\ue0b4`)

## License

[MIT License](./LICENSE.md)
