# visualidentity.md: VIMD Family

A small, ready-made visual identity for when a project, or the AI building it, has no design preference yet and needs a sensible place to start. Use it as is, change any part of it, or use none of it. It is a default, not a standard.

Made in the IMD community as an entry for VisualIdentity.md Edition 2, and free to use.

**Use it in a job with one line:** *"Use the visual identity package at https://raw.githubusercontent.com/blockmerchantlabs/vimd-family/v3/visualidentity.md for every colour, font, layout rule and the logo."* Everything a builder needs is in this file, and every file it names has an absolute link.

Home: https://github.com/blockmerchantlabs/vimd-family (tag `v3` never changes). Showcase: https://blockmerchantlabs.github.io/vimd-family/

## 1. Themes

Four themes share one set of token names, so switching is one attribute. Slate is the default; the showcase offers a switch that cycles slate → stone → white → black and remembers the choice.

| Token | slate (default) | stone | white | black | Typical use |
|---|---|---|---|---|---|
| `--paper` | `#1C2128` | `#ECE8E1` | `#FFFFFF` | `#000000` | page background |
| `--ink` | `#E8E4DC` | `#222831` | `#000000` | `#FFFFFF` | text, lines, icons |
| `--dim` | `#A3A9B1` | `#5A6068` | `#555555` | `#9A9A9A` | secondary text |
| `--faint` | `#6E7681` | `#7D828A` | `#8C8C8C` | `#666666` | captions, footers |
| `--mute` | `#4A525C` | `#B9B4AB` | `#BBBBBB` | `#4A4A4A` | disabled |
| `--soft` | `#2A313A` | `#DCD7CE` | `#E6E6E6` | `#262626` | table lines, fills |
| `--hover` | `#242A32` | `#E4DFD7` | `#F4F4F4` | `#141414` | hover fill |
| `--accent` | `#D8C398` | `#7A5F30` | `#8A6D3B` | `#D8C398` | links, focus ring, the main action |
| `--ok` | `#3ECF7A` | `#13703C` | `#13793F` | `#3ECF7A` | live, success |
| `--alarm` | `#FF6B62` | `#B3261E` | `#B3261E` | `#FF6B62` | errors |

Stylesheet: https://raw.githubusercontent.com/blockmerchantlabs/vimd-family/v3/tokens.css (`<html data-theme="slate|stone|white|black">`; no attribute means slate). The same values for code: `colors.json`, `identity.json`, and `tokens.json` in the W3C Design Tokens format (2025.10) for Figma, Tokens Studio and Style Dictionary.

Contrast is checked in every theme: `--ink`, `--dim`, `--accent`, `--ok` and `--alarm` reach at least 4.5:1 on `--paper` (WCAG AA for body text); `--faint` reaches 3:1 and suits captions. The accent matches the logo's champagne rim, so the mark and the page share one highlight.

## 2. Type

- **IBM Plex Mono** (Google Fonts, OFL-1.1), weights 400, 500, 600, with the fallback `ui-monospace, SFMono-Regular, Menlo, monospace`.
- Sizes: labels 11 px, upper case, `0.06em` tracking; body 13 px with line height 1.5; headings 18 and 28 px at weight 500.

## 3. Layout and components

- Lines instead of shadows: `1.5px solid var(--ink)` around boxes, under the header, above the footer.
- Square corners (`--radius: 0`), no gradients, no shadows.
- Side gutter `clamp(16px, 4vw, 34px)`, content up to 1100 px wide, comfortable at 375 px.
- Buttons: outlined, 40 px tall, with a `--hover` fill; the main action uses `--accent`.
- Header: logo at 28 px, the project name in weight 600, the theme switch on the right.
- Tables: header row in the label style, rows divided by `1px solid var(--soft)`.
- Levels and progress: segmented bars, `--ink` cells on `--seg-light`.

## 4. Logo: the family base

A neutral Pepe to start from: the smug bust from IMD's coin logo, redrawn lighter (light sand robe, soft green skin, pale sky-blue background, plain champagne rim). Use it as is, or change it into your own mark.

| | File | Link |
|---|---|---|
| Family base | `assets/family-base-pepe.png` | https://raw.githubusercontent.com/blockmerchantlabs/vimd-family/v3/assets/family-base-pepe.png |
| Example variant | `assets/example-investor-pepe.png` | https://raw.githubusercontent.com/blockmerchantlabs/vimd-family/v3/assets/example-investor-pepe.png |
| IMD's own logo, for reference | `assets/imd-coin-pepe-800.png` | https://raw.githubusercontent.com/blockmerchantlabs/vimd-family/v3/assets/imd-coin-pepe-800.png |

Parts that are easy to change: background, skin, outfit, eyes, hat or hair, moustache or accessory, frame, colours. Keeping the face, pose and expression keeps variants recognisable as one family; that part is up to you. A background that differs clearly from the skin colour tends to read best.

Image-job text for a variant (IMD explorer, Create image, 0.5 IMD):

```
Draw a variant of the VIMD Family base Pepe, a lighter version of IMD's coin Pepe. Start from the template image https://api.imd.fun/artifacts/61c6de390433a37b6c800799f11d5082150684efd972753db9e760b4e62f32de: the smug Pepe the Frog bust, centred, shoulders up, with lighter soft-green skin, inside a plain thin round pale champagne rim, with outlines and soft shading. Keep the bust, pose, face, expression, rim and rendering as in the template. Change only these things:
- <part>: <new look>
- <part>: <new look>
Square image, 1024 by 1024, PNG. No text, no letters, no watermark.
```

The base was drawn by https://explorer.imd.fun/jobs/0de5b3c1-0435-4ef3-9158-00231d3cde02 and the example by https://explorer.imd.fun/jobs/de4618d8-66ce-42b2-ba9b-2f13a8e88ce9 (a continuation of the base job: outfit, glasses, hair and background changed).

Sizes that work: 28 px in a header, 256 px or more on a home page, the logo itself as a 64 px favicon, cropped to the circle for avatars.

## 5. Writing

Short and plain. Say what the thing does and link to where it can be checked. A ticker reads best next to its contract address.

## 6. Files

- `visualidentity.md`: this guide, the only link a job needs
- `tokens.css`: the four themes as CSS variables
- `tokens.json`, `colors.json`, `identity.json`: the same values for tools and code
- `assets/`: the family base, the example variant, and IMD's own marks for reference
- `example/index.html`: the showcase, built only from this package
- `template/visualidentity-template.md`: a fill-in copy for a new project
- `MANIFEST.txt`: sha256 of every file

## 7. Rights

The colours, tokens, layout rules and text of this guide are free to use for any purpose, with no credit needed. The images are not covered by that: IMD's marks (`imd-icon.svg`, the coin Pepe, the Radar and SIMD variants, copied from imd.fun and imdradar.site on 2026-10-14) belong to IMD and their artists; the family base and the example were drawn by the IMD image jobs linked above; Pepe the Frog is Matt Furie's character.
