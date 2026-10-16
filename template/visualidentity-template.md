# visualidentity.md template: a project in the IMD style

Copy this file next to a copy of this package, fill in every `<…>`, and keep the rest. A project built from it reads as part of IMD: same paper and ink, same type, same rules, and a mark that is the IMD coin Pepe with one change.

## 1. Project

- Name: `<project name>`
- One line: `<what it does, in under 12 words>`
- Launch record: `<IMD launch number or contract address, once it exists>`
- Ticker: leave empty until the contract exists, and always show it with the contract address.

## 2. Mark

Start from the family base, `../assets/family-base-pepe.png` (drawn by IMD image job https://explorer.imd.fun/jobs/0de5b3c1-0435-4ef3-9158-00231d3cde02, image https://api.imd.fun/artifacts/61c6de390433a37b6c800799f11d5082150684efd972753db9e760b4e62f32de). It is IMD's coin Pepe in a light, neutral palette: IMD's own gold coin stays IMD's. Keep the bust, pose, face and expression. Change any of these slots, and name them:

| Slot | Family base | This project |
|---|---|---|
| Background | pale pastel sky blue | `<keep / change to …>` |
| Skin | lighter soft green | `<keep / change to …>` |
| Outfit | light sand robe, pale tan underlayer | `<keep / change to …>` |
| Eyes | smug eyes | `<keep / change to …>` |
| Hat / hair | nothing | `<keep / change to …>` |
| Moustache / accessory | nothing | `<keep / change to …>` |
| Frame | plain thin round rim, pale champagne | `<keep / change to …>` |

Keep the background and the skin clearly different colours.

Examples already in use: IMD Radar (black suit and tie, cyborg eye with red laser, green radar ring); SIMD (Einstein hair, white coat, line art).

Request text for an IMD image job (0.5 IMD), with your changes filled in (run it as a continuation of the base job if you paid for it, or as a new job):

```
Draw a variant of the neutral default IMD coin Pepe. Start from the template image https://api.imd.fun/artifacts/61c6de390433a37b6c800799f11d5082150684efd972753db9e760b4e62f32de: the smug Pepe the Frog bust, centred, shoulders up, with lighter soft-green skin, inside a plain thin round pale champagne rim, in IMD's coin-art rendering with outlines and soft shading. Keep the bust, pose, face, expression, rim and rendering exactly as in the template. Change only these things:
- <slot>: <new trait>
- <slot>: <new trait>
Square image, 1024 by 1024, PNG. No text, no letters, no watermark.
```

## 3. Colour, type, layout, voice

Use `../tokens.css` as is: default theme slate, switch to stone, white or black. Optional: set your own `--accent: <hex>` (one highlight per screen); keep every other token.

Type stays IBM Plex Mono. Rules stay `1.5px solid`. Square corners, no gradients, no shadows.

In an IMD job, one line does all of this: "Use the visual identity package at https://raw.githubusercontent.com/blockmerchantlabs/vimd2-imd-official/v2/visualidentity.md for every colour, font, layout rule and the logo."

## 4. Check before publishing

- The page built from `../example/index.html` with your mark swapped in still looks like the IMD Family showcase.
- The mark's face is unchanged.
- No ticker without its contract address next to it.
