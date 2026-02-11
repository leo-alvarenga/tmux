# Tmux

A maintainable, **dependency-free** _[tmux](https://github.com/tmux/tmux)_ config that separates core behavior from styling using sourced `.conf` files simple to extend, easy to style.

> Make sure to also check my Neovim configuration, which is designed to work seamlessly with this Tmux setup: [leo-alvarenga/nvim](https://github.com/leo-alvarenga/nvim)

## Setup

To setup and use this configuration run this command:

```bash
git clone https://github.com/leo-alvarenga/tmux "$HOME/.config/tmux"
```

## Theming

You can change the theme by sourcing a different `.conf` file in `./tmux.conf`:

```conf
## Theme
source-file "$HOME/.config/tmux/onedark.conf"

# Or
# source-file "$HOME/.config/tmux/YOUR_THEME.conf"
```

You can also create your own theme by copying one of the existing ones and modifying it to your liking.

### Available Themes

These are the themes available in this repository:

- [Catppuccin Mocha](./catppuccin.conf)
- [One Dark](./onedark.conf)

## License

[MIT License](./LICENSE.md)
