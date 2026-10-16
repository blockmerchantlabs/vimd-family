# visualidentity.md: IMD Family

Entry for VisualIdentity.md Edition 2. One complete visual identity for any project in the IMD ecosystem: in IMD's style without copying IMD. IMD keeps its own white-and-black site and its gold coin; the family uses stone and slate and a lighter base Pepe.

**How to use it in a job:** add one line, for example: *"Use the visual identity package at https://raw.githubusercontent.com/blockmerchantlabs/vimd2-imd-official/v2/visualidentity.md for every colour, font, layout rule and the logo."* Everything a builder needs is in this file; every file it names has an absolute link.

Package home: https://github.com/blockmerchantlabs/vimd2-imd-official (tag `v2`, which never changes). Showcase: https://blockmerchantlabs.github.io/vimd2-imd-official/

## 1. Themes

Four themes, one set of token names. **Default: slate.** A site offers a theme switch that cycles slate → stone → white → black and remembers the choice.

| Token | slate (default) | stone | white | black | Use |
|---|---|---|---|---|---|
| `--paper` | `#1C2128` | `#ECE8E1` | `#FFFFFF` | `#000000` | page ground |
| `--ink` | `#E8E4DC` | `#222831` | `#000000` | `#FFFFFF` | text, rules, icons |
| `--dim` | `#A3A9B1` | `#5A6068` | `#555555` | `#9A9A9A` | secondary text |
| `--faint` | `#6E7681` | `#7D828A` | `#8C8C8C` | `#666666` | captions, footers (non-essential, ≥3:1) |
| `--mute` | `#4A525C` | `#B9B4AB` | `#BBBBBB` | `#4A4A4A` | disabled |
| `--soft` | `#2A313A` | `#DCD7CE` | `#E6E6E6` | `#262626` | table lines, fills |
| `--hover` | `#242A32` | `#E4DFD7` | `#F4F4F4` | `#141414` | hover fill |
| `--accent` | `#D8C398` | `#7A5F30` | `#8A6D3B` | `#D8C398` | links, focus ring, one highlight per screen |
| `--ok` | `#3ECF7A` | `#13703C` | `#13793F` | `#3ECF7A` | live, success |
| `--alarm` | `#FF6B62` | `#B3261E` | `#B3261E` | `#FF6B62` | errors only |

Stylesheet with all four: https://raw.githubusercontent.com/blockmerchantlabs/vimd2-imd-official/v2/tokens.css (set `<html data-theme="slate|stone|white|black">`; no attribute means slate). Machine-readable: `colors.json`, `identity.json`, and `tokens.json` (W3C Design Tokens format).

Colour means state: green live, red alarm, accent for the one thing to click. Everything else is paper and ink.

Contrast, checked for every theme: `--ink`, `--dim`, `--accent`, `--ok` and `--alarm` are at least 4.5:1 on `--paper` (WCAG AA for body text); `--faint` is at least 3:1 and is only for captions. The accent is the colour of the logo's champagne rim, so the mark and the interface share one highlight.

## 2. Type

- One family: **IBM Plex Mono** (Google Fonts, OFL-1.1), weights 400, 500, 600. Fallback `ui-monospace, SFMono-Regular, Menlo, monospace`.
- Sizes: labels 11 px upper case with `0.06em` tracking; body 13 px, line height 1.5; headings 18 and 28 px at weight 500.
- Numbers before adjectives. Lower case where it reads naturally.

## 3. Layout and components

- Rules, not shadows: `1.5px solid var(--ink)` around boxes, under the header, above the footer.
- Square corners everywhere (`--radius: 0`). No gradients, no drop shadows, no blur.
- Side gutter `clamp(16px, 4vw, 34px)`; content max width 1100 px; works at 375 px wide.
- Buttons: outlined pills 40 px tall, `--ink` border, `--hover` fill on hover; the primary action uses `--accent` for its border and text.
- Header: logo at 28 px, project name in weight 600 with tracking, theme switch on the right.
- Tables: header row in label style; rows separated by `1px solid var(--soft)`.
- Instruments: segmented bars (cells of `--ink` on `--seg-light`) for levels and progress.

## 4. Logo: the family base Pepe

Every project's mark is the **family base** with its own changes. IMD's gold-coin Pepe belongs to IMD and is not used by family projects.

| | File | Link |
|---|---|---|
| Family base (start here) | `assets/family-base-pepe.png` | https://raw.githubusercontent.com/blockmerchantlabs/vimd2-imd-official/v2/assets/family-base-pepe.png |
| Example project | `assets/example-investor-pepe.png` | https://raw.githubusercontent.com/blockmerchantlabs/vimd2-imd-official/v2/assets/example-investor-pepe.png |
| IMD's own mark (parent, IMD only) | `assets/imd-coin-pepe-800.png` | https://raw.githubusercontent.com/blockmerchantlabs/vimd2-imd-official/v2/assets/imd-coin-pepe-800.png |

The family base: the smug Pepe bust from IMD's coin, same pose, face and expression, in a light sand robe, lighter soft-green skin, pale sky-blue ground, inside a plain thin champagne rim, no stars. Drawn by IMD image job https://explorer.imd.fun/jobs/0de5b3c1-0435-4ef3-9158-00231d3cde02.

**What a project changes:** background colour, skin colour, outfit, eyes, hat or hair, moustache or accessory, frame, colours. **What never changes:** the face, pose and expression. Keep background and skin clearly different colours.

Image-job text to make a project's mark (IMD explorer, Create image, 0.5 IMD):

```
Draw a variant of the neutral default IMD coin Pepe. Start from the template image https://api.imd.fun/artifacts/61c6de390433a37b6c800799f11d5082150684efd972753db9e760b4e62f32de: the smug Pepe the Frog bust, centred, shoulders up, with lighter soft-green skin, inside a plain thin round pale champagne rim, in IMD's coin-art rendering with outlines and soft shading. Keep the bust, pose, face, expression, rim and rendering exactly as in the template. Change only these things:
- <part>: <new look>
- <part>: <new look>
Square image, 1024 by 1024, PNG. No text, no letters, no watermark.
```

The example project was made exactly this way (outfit, glasses, hair, background changed): https://explorer.imd.fun/jobs/de4618d8-66ce-42b2-ba9b-2f13a8e88ce9.

Logo use: show it at 28 px in the header and 256 px or larger on the home page; crop to the circle for avatars; favicon is the logo at 64 px. Never add text inside the logo.

## 5. Voice

Terse, technical, plain. Say what the contract does and link the record. A ticker appears only next to its contract address.

## 6. Files

- `visualidentity.md`: this guide (the one link a job needs)
- `tokens.css`: the four themes as CSS variables
- `colors.json`, `identity.json`: the same values for code
- `tokens.json`: the same tokens in the W3C Design Tokens format (2025.10), for Figma, Tokens Studio and Style Dictionary
- `assets/`: family base, example project, and IMD's own marks for reference (`imd-icon.svg`, `imd-coin-pepe-*.png`, Radar and SIMD variants)
- `example/index.html`: the showcase, built only from this package, slate by default
- `template/visualidentity-template.md`: fill-in copy for a new project
- `MANIFEST.txt`: sha256 of every file

## 7. Provenance and rights

IMD's marks (`imd-icon.svg`, the coin Pepe, Radar and SIMD variants) were copied on 2026-10-14 from imd.fun and imdradar.site and belong to IMD and their artists. The family base and the example were drawn by IMD image jobs linked above. Pepe the Frog is Matt Furie's character. This package claims no ownership and grants no licence over those marks; the colours, layout rules and text of this guide are offered for anyone in the IMD community to use.
