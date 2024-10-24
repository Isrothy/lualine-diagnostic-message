# lualine-diagnostic-message

Show LSP diagnostic message on lualine

## Screenshot

<img width="1438" alt="image" src="https://user-images.githubusercontent.com/61075605/213876470-98d47e09-16fc-4994-88e0-550dffc32a1a.png">

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
            --- If you want to custoimze the colors
            colors = {
                error = "#BF616A",
                warn = "#EBCB8B",
                info = "#A3BE8C",
                hint = "#88C0D0",
            },
            --- If you want to custoimze the icons
            icons = {
                error = "E",
                warn = "W",
                info = "I",
                hint = "H",
            }
            -- Replace '\n' by the separator
            line_separator = ". ",

            -- Only show the first line of diagnostic message
            first_line_only = false,
        }
    }
}
```
