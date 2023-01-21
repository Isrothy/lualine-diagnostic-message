# lualine-diagnostic-message

Show LSP diagnostic message on lualine

## Screenshot

## Installation

[packer.nvim](https://github.com/wbthomason/packer.nvim)

```lua
use 'Isrothy/lualine-diagnostic-message'
```

[lazy](https://github.com/folke/lazy.nvim)

```lua
{
  "Isrothy/lualine-diagnostic-message",
}
```

## Use

```lua
require'lualine'.setup{
    sections = {
        lualine_c = {
            "diagnostic-message",
            --- If you want to custoimze the color
            colors = {
                error = "#BF616A",
                warn = "#EBCB8B",
                info = "#A3BE8C",
                hint = "#88C0D0",
            }
        }
    }
}
```
