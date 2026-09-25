# Noctis

![Variants preview][img-preview]

Color schemes for [Sublime Text](https://www.sublimetext.com/), powered by the
beautiful [Noctis][noctis] theme by Liviu Shera. Started as a fork of the
[Timeless][timeless] theme by Ricci Adams.

## Highlights

* **11 color schemes** — 8 dark and 3 light variants of the Noctis palette.

* **Faithful port** of the syntax token colors from the original VS Code theme.

* Editor colors included — caret, selection, line highlight, indent guides,
  find matches and the active line number are themed per variant.

* **Works with every UI theme** — color schemes are independent of the
  `.sublime-theme` in use.

* Each scheme exposes its full palette through named `variables`, so you can
  tweak colors without touching the rules.

## Variants

| Color Scheme | Type | Background |
| ------------ | ---- | ---------- |
| `Noctis` | dark | very saturated very dark cold bluish cyan |
| `Noctis Azureus` | dark | very saturated very dark cold azure |
| `Noctis Bordo` | dark | very unsaturated very dark warm rose |
| `Noctis Minimus` | dark | Azureus palette with much lower saturation |
| `Noctis Obscuro` | dark | darker variant of the Noctis palette |
| `Noctis Sereno` | dark | brighter variant of the Noctis palette |
| `Noctis Uva` | dark | unsaturated dark cold blue |
| `Noctis Viola` | dark | saturated very dark cold violet |
| `Noctis Hibernus` | light | very unsaturated very light cold bluish cyan |
| `Noctis Lilac` | light | very unsaturated very light cold blue |
| `Noctis Lux` | light | very saturated very light warm orange |

## Installation

### Package Control

The package is listed as `Noctis Color Scheme`:

1. Open `Command Palette` using menu item `Tools → Command Palette...`
2. Choose `Package Control: Install Package`
3. Find `Noctis Color Scheme` and hit `Enter`

### Git clone

1. Open the `Packages` directory via menu item `Preferences → Browse Packages...`
2. Clone the repository into it:

   ```bash
   git clone https://github.com/ziishaned/sublime-text-noctis.git "Noctis"
   ```

3. Restart Sublime Text.

## Activation

Pick a variant via `Preferences → Select Color Scheme...`, or set it in your
user preferences:

```json
{
    "color_scheme": "Packages/Noctis/Noctis.sublime-color-scheme"
}
```

## Customization

Every scheme defines its palette as named `variables`. To adjust colors, create
a `Noctis Custom.sublime-color-scheme` in your `User` package that extends a
variant and override just what you want:

```json
{
    "extends": "Packages/Noctis/Noctis.sublime-color-scheme",
    "variables": {
        "background": "#041d20",
        "comment": "#6fa3a3"
    }
}
```

## Acknowledgments

* [Noctis][noctis] by Liviu Shera — the color palette every scheme in this
  package is generated from (MIT License)
* [Timeless][timeless] by Ricci Adams — this repository started as a fork of
  the Timeless theme before it was reduced to the color schemes
  (public domain, [CC0 1.0][cc0])

## License

[MIT](LICENSE.md)

<!-- Links -->

[noctis]: https://github.com/liviuschera/noctis
[timeless]: https://github.com/iccir/Timeless-Theme
[cc0]: https://creativecommons.org/publicdomain/zero/1.0/

<!-- Assets -->

[img-preview]: media/preview.png
