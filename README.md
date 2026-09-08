<p align="center">
  <img src="assets/logo.svg" alt="code-2026" width="96" />
</p>

<p align="center">
  <img src="assets/yazi.png" alt="code-2026" />
</p>

# code-2026.yazi

Yazi flavors based on VS Code's **Dark Modern 2026** theme — red keywords, purple functions,
teal types and light-blue strings. Available in dark and light variants.

## The code-2026 family

| Target  | Repository                                                            |                |
| ------- | --------------------------------------------------------------------- | -------------- |
| Neovim  | [code-2026-theme/nvim](https://github.com/code-2026-theme/nvim)       | colorscheme    |
| Ghostty | [code-2026-theme/ghostty](https://github.com/code-2026-theme/ghostty) | terminal theme |
| kitty   | [code-2026-theme/kitty](https://github.com/code-2026-theme/kitty)     | terminal theme |
| Xcode   | [code-2026-theme/xcode](https://github.com/code-2026-theme/xcode)     | editor theme   |
| Obsidian | [code-2026-theme/obsidian](https://github.com/code-2026-theme/obsidian) | app theme    |
| Yazi    | [code-2026-theme/yazi](https://github.com/code-2026-theme/yazi)       | **this repo**  |

Every port shares one palette, so your file manager and editor match exactly.

## Features

- Full coverage of all yazi UI elements: manager, tabs, mode, status bar, which, confirm,
  spot, notify, pick, input, completion, tasks, help, and filetype rules.
- Semantic file-type coloring by MIME type.
- Custom icon rules for directories, executables, symlinks, and special files.

## Requirements

- [Yazi](https://yazi-rs.github.io) v0.2.4+

## Installation

```bash
# Via ya package manager
ya pkg add yazi-rs/flavors:code-2026
```

Or use the install script:

```sh
./install.sh
```

Or clone manually:

```bash
git clone https://github.com/code-2026-theme/yazi ~/.config/yazi/flavors/code-2026.yazi
```

## Usage

Set the content of your `~/.config/yazi/theme.toml`:

```toml
[flavor]
dark = "code-2026"
# or for the light variant:
dark = "light-2026"
```

Make sure your `theme.toml` doesn't contain anything other than `[flavor]`, unless you want
to override certain styles of this flavor.

## Customization

Override specific styles in your `theme.toml` after the `[flavor]` section:

```toml
[flavor]
dark = "code-2026"

[mgr]
cwd = { fg = "#4ec9b0" }

[status]
perm_write = { fg = "#ffa657" }
```

## Palette

| Key          | Value     | Role                       |
| ------------ | --------- | -------------------------- |
| `bg`         | `#121314` | editor background          |
| `bg_alt`     | `#191a1b` | panels, inactive tabs      |
| `bg_menu`    | `#202122` | floats, popups             |
| `border`     | `#2a2b2c` | window separators          |
| `border_alt` | `#333536` | float borders              |
| `fg`         | `#bbbebf` | default text               |
| `fg_dim`     | `#8c8c8c` | secondary text             |
| `fg_muted`   | `#555555` | line numbers, whitespace   |
| `accent`     | `#3994bc` | cwd, borders, status       |
| `keyword`    | `#ff7b72` | cut markers, errors        |
| `func`       | `#d2a8ff` | archives, purple elements  |
| `type`       | `#4ec9b0` | select mode, images        |
| `string`     | `#a5d6ff` | light blue accents         |
| `annotation` | `#ffa657` | unset mode, permissions    |
| `constant`   | `#79c0ff` | blue accents               |
| `ok`         | `#7ee787` | copied markers, success    |
| `warn`       | `#cd9731` | selected markers, warnings |
| `err`        | `#ff7b72` | error states               |
| `comment`    | `#8b949e` | muted text                 |
| `debug`      | `#b267e6` | debug elements             |

### Light palette

| Key          | Value     | Role                       |
| ------------ | --------- | -------------------------- |
| `bg`         | `#FFFFFF` | editor background          |
| `bg_alt`     | `#FAFAFD` | panels, inactive tabs      |
| `bg_menu`    | `#FAFAFD` | floats, popups             |
| `border`     | `#F0F1F2` | window separators          |
| `border_alt` | `#E4E5E6` | float borders              |
| `fg`         | `#202020` | default text               |
| `fg_dim`     | `#606060` | secondary text             |
| `fg_muted`   | `#999999` | line numbers, whitespace   |
| `accent`     | `#0069CC` | cwd, borders, status       |
| `keyword`    | `#cf222e` | cut markers, errors        |
| `func`       | `#8250df` | archives, purple elements  |
| `type`       | `#116329` | select mode, images        |
| `string`     | `#0a3069` | dark blue accents          |
| `annotation` | `#953800` | unset mode, permissions    |
| `constant`   | `#0550ae` | blue accents               |
| `ok`         | `#587c0c` | copied markers, success    |
| `warn`       | `#667309` | selected markers, warnings |
| `err`        | `#ad0707` | error states               |
| `comment`    | `#6e7781` | muted text                 |
| `debug`      | `#8250df` | debug elements             |

## License

[MIT](LICENSE)
