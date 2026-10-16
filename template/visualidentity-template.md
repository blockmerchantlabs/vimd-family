# visualidentity.md template: start from the VIMD Family

A fill-in copy for a project that wants to start from the VIMD Family. Fill in the `<…>` parts you need, keep what suits you, and change the rest.

## 1. Project

- Name: `<project name>`
- One line: `<what it does, in under 12 words>`
- Launch record: `<IMD launch number or contract address, once it exists>`
- Ticker: `<optional; reads best next to the contract address>`

## 2. Mark

Start from the family base, `../assets/family-base-pepe.png` (drawn by IMD image job https://explorer.imd.fun/jobs/0de5b3c1-0435-4ef3-9158-00231d3cde02, image https://api.imd.fun/artifacts/61c6de390433a37b6c800799f11d5082150684efd972753db9e760b4e62f32de). It is a lighter version of IMD's coin Pepe. Change any of these parts:

| Part | Family base | This project |
|---|---|---|
| Background | pale pastel sky blue | `<keep / change to …>` |
| Skin | lighter soft green | `<keep / change to …>` |
| Outfit | light sand robe, pale tan underlayer | `<keep / change to …>` |
| Eyes | smug eyes | `<keep / change to …>` |
| Hat / hair | nothing | `<keep / change to …>` |
| Moustache / accessory | nothing | `<keep / change to …>` |
| Frame | plain thin round rim, pale champagne | `<keep / change to …>` |

A background that differs clearly from the skin tends to read best.

Other Pepe variants in the IMD community, for ideas: IMD Radar (black suit and tie, cyborg eye with red laser, green radar ring); SIMD (Einstein hair, white coat, line art).

Request text for an IMD image job (0.5 IMD), with your changes filled in (run it as a continuation of the base job if you paid for it, or as a new job):

```
Draw a variant of the VIMD Family base Pepe, a lighter version of IMD's coin Pepe. Start from the template image https://api.imd.fun/artifacts/61c6de390433a37b6c800799f11d5082150684efd972753db9e760b4e62f32de: the smug Pepe the Frog bust, centred, shoulders up, with lighter soft-green skin, inside a plain thin round pale champagne rim, with outlines and soft shading. Keep the bust, pose, face, expression, rim and rendering as in the template. Change only these things:
- <part>: <new look>
- <part>: <new look>
Square image, 1024 by 1024, PNG. No text, no letters, no watermark.
```

## 3. Colour, type, layout

`../tokens.css` gives four themes (slate by default, stone, white, black). Common changes: your own `--accent: <hex>`, a different default theme, or your own font. Change as much or as little as you like.

In a job, one line brings in the whole package: "Use the visual identity package at https://raw.githubusercontent.com/blockmerchantlabs/vimd-family/v3/visualidentity.md for every colour, font, layout rule and the logo."

## 4. Quick check (optional)

- Swap your mark into `../example/index.html` to preview it in all four themes.
- The mark still reads at 28 px.
- A ticker, if any, sits next to its contract address.
