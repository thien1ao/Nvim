# Neovim Config

My personal Neovim setup, written in Lua and managed with [lazy.nvim](https://github.com/folke/lazy.nvim).

## Screenshots

![Neovim screen](assets/nvim_screen.png)

![Neovim example](assets/nvim_ex.png)

## Features

- Colorscheme: [darkvoid.nvim](https://github.com/aliqyan-21/darkvoid.nvim)
- Fuzzy finding with `fzf` and `telescope.nvim`
- LSP support via `nvim-lspconfig`, plus custom snippets in `my_lsp_snips/`
- LaTeX with `vimtex`
- Arduino support via `Arduino-Nvim`
- File explorer with NvimTree (`<leader>n`)
- Per-filetype settings in `ftplugin/` (C, C++, Python, Rust, Lua, Fortran, TeX, Markdown, ...)

## Structure

```
.
├── init.lua          # core settings and keymaps
├── lua/
│   ├── config.lua    # plugin configuration
│   └── plugins.lua   # plugin list
├── ftplugin/         # filetype-specific settings
├── my_lsp_snips/     # custom snippets
├── assets/           # screenshots
└── lazy-lock.json
```

## Key mappings

Leader key is `,`.

| Key | Mode | Action |
| --- | --- | --- |
| `jj` / `jk` / `jw` | insert | Exit insert mode |
| `<Space>` | normal | Insert a single character |
| `<Tab>` / `<S-Tab>` | normal | Next / previous buffer |
| `<C-e>` | normal | List buffers and switch |
| `<C-h/j/k/l>` | normal | Move between windows |
| Arrow keys | all | Resize windows |
| `<leader>s` | normal | Replace word under cursor |
| `<leader>tn` / `<leader>tm` | normal | Previous / next tab |
| `<leader>n` | normal | Open file tree |
| `<C-c>` | visual | Copy to system clipboard |

## Installation

```sh
git clone https://github.com/thien1ao/nvim ~/.config/nvim
nvim
```

Plugins are installed automatically on first launch.
