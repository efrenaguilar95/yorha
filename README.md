# YoRHa

An [Omarchy](https://omarchy.org/) theme inspired by the YoRHa faction from
*NieR: Automata* — specifically the game's in-game menu UI: aged
parchment/beige surfaces, dark ink-toned text, and deep red highlight accents,
overlaid here with an original HUD-style schematic (grid, targeting rings, and
corner tick marks) rather than any reproduced game art. It is a **light**
theme. A dark theme based on the androids' black-and-white uniforms is planned
as a separate companion theme.

This is a fan-made, unofficial theme not affiliated with Square Enix or
PlatinumGames. All artwork (the background, preview images) is original,
created procedurally — no game assets are included.

## Install

```bash
omarchy theme install <this-repo-url>
omarchy theme set yorha
```

Note: Omarchy derives a theme's *displayed* name mechanically from its
directory/repo slug (capitalizing only the first letter), so `omarchy theme
current`/`list` will show this as "Yorha" rather than the lore-accurate
"YoRHa" spelling used here and in this README.

## Palette

See [`colors.toml`](colors.toml) for the full palette. Highlights:

| Role | Color |
|---|---|
| Background (parchment) | `#e8dcc0` |
| Foreground (ink) | `#2b2620` |
| Accent (YoRHa red) | `#a13d2f` |
| Gold trim | `#b8942f` |

## Font

Recommended: **AdwaitaMono Nerd Font Mono**. The in-game UI (see
[reference](https://interfaceingame.com/wp-content/uploads/nierautomata/nierautomata-items.jpg))
uses a clean geometric sans with no serifs — reportedly
[Rodin](https://en.fontworks.co.jp/case/10971/), a proprietary Japanese
typeface, so not something we can ship or install directly. Of the free,
officially-packaged Nerd Fonts tried, Adwaita Mono was the only one whose
`T`/`I`/`l`/`1` came out serif-free at terminal sizes — JetBrainsMono,
Monaspace Xenon, IBM Plex Mono (BlexMono), and Monaspace Neon all carry small
slab-serif ticks that read further from the reference than they first
appear.

```bash
omarchy pkg add ttf-adwaitamono-nerd
omarchy font set "AdwaitaMono Nerd Font Mono"
```

Use the `Mono` variant specifically — it's the one with icon glyphs patched
to a single monospace cell, which keeps waybar/omarchy-shell icons aligned.
The plain `AdwaitaMono Nerd Font` and `AdwaitaMono Nerd Font Propo` variants
size icons differently and can throw off terminal/bar alignment.

## License

MIT — see [LICENSE](LICENSE).
