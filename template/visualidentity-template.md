# visualidentity.md template: a project in the IMD style

Copy this file next to a copy of this package, fill in every `<…>`, and keep the rest. A project built from it reads as part of IMD: same paper and ink, same type, same rules, and a mark that is the IMD coin Pepe with one change.

## 1. Project

- Name: `<project name>`
- One line: `<what it does, in under 12 words>`
- Launch record: `<IMD launch number or contract address, once it exists>`
- Ticker: leave empty until the contract exists, and always show it with the contract address.

## 2. Mark

Start from `../assets/imd-coin-pepe-800.png`. Keep the bust, pose, face and expression. Change one or two traits only, and name them:

| Slot | IMD base | This project |
|---|---|---|
| Outfit | orange robe | `<keep / change to …>` |
| Eyes | smug eyes | `<keep / change to …>` |
| Head | nothing | `<keep / change to …>` |
| Accessory | nothing | `<keep / change to …>` |
| Frame | gold coin with stars | `<keep / change to …>` |
| Ground | royal blue | `<keep / change to …>` |

Examples already in use: IMD Radar (black suit and tie, cyborg eye with red laser, green radar ring); SIMD (Einstein hair, white coat, line art).

Request text for an IMD image job (0.5 IMD), with your traits filled in:

```
Draw the IMD coin Pepe: the smug Pepe the Frog bust from IMD's coin logo, same pose, same face and expression, centred, shoulders up. Keep IMD's coin-art rendering: clean outlines, flat colour, soft shading. Change only these traits:
- <slot>: <new trait>
- <slot>: <new trait>
Square image, 1024 by 1024, PNG. No text, no letters, no watermark.
```

## 3. Colour, type, layout, voice

Use `../tokens.css` as is. Optional: one accent colour for the project's state colour, `--accent: <hex>`, used only where IMD uses green.

Type stays IBM Plex Mono. Rules stay `1.5px solid`. Square corners, no gradients.

## 4. Check before publishing

- The page built from `../example/index.html` with your mark swapped in still looks like imd.fun.
- The mark's face is unchanged.
- No ticker without its contract address next to it.
