# visualidentity.md: IMD, as it is today

Entry for VisualIdentity.md Edition 2. This package is not a new design. It records the look IMD already uses on imd.fun, on its coin, and on IMD Radar, so that the default is IMD itself and every later edition starts from here.

**Default outcome:** a page built from this file at its defaults comes out as the IMD site: monochrome paper and ink, IBM Plex Mono, 1.5 px rules, the diamond mark in the header, and the IMD Pepe as the face. `example/index.html` is that page, built only from `tokens.css` and the files in `assets/`.

## 1. Marks

| Mark | File | Use |
|---|---|---|
| Diamond mark | `assets/imd-icon.svg` (from imd.fun/icon.svg) | Logo, favicon, header. White square, black 3 px border, black diamond outline. On dark ground it inverts: black square, white diamond. |
| App icon | `assets/imd-app-icon.png`, `assets/imd-favicon.ico` | Home-screen and browser tab. |
| IMD Pepe (coin) | `assets/imd-coin-pepe-256.png`, `assets/imd-coin-pepe-800.png` | The face of IMD: the smug Pepe bust in an orange robe over brown, on royal blue, inside a gold coin rim with stars. Token logo, avatar, social. |
| Walking Pepe | `assets/imd-site-pepe-walk.webp` (19 frames, 240 px tall) | Motion on the site. Classic Pepe, blue shirt, brown shorts. |
| Share card | `assets/imd-share-card.png` | Link previews: terminal and instrument dials. |

Rules: never redraw the diamond; keep clear space of one diamond-width around it; the Pepe bust keeps its pose, face and expression in every use.

## 2. The Pepe variant system

IMD's ecosystem already extends the mascot by changing traits on the same bust:

| Variant | File | Same | Changed |
|---|---|---|---|
| IMD (base) | `imd-coin-pepe-256.png` | bust, pose, smug eyes, lip, chin | orange robe, blue ground, gold star coin |
| IMD Radar | `imdradar-pepe-variant.jpg` | bust, pose, face | black suit and tie, cyborg eye piece with red laser, green radar ring |
| SIMD (Superintelligent Identity.md) | `simd-pepe-variant.jpg` | bust, pose, star-coin frame | Einstein hair and moustache, white coat and tie, line art |

A new project's mark is the base bust with its own traits: clothing, eyewear, hair or headwear, frame, ground, rendering style. One or two traits carry the idea; the face never changes.

## 3. Colour

Monochrome first. Colour means state: green is live or OK, red is alarm.

| Token | Light | Dark |
|---|---|---|
| `--paper` (ground) | `#ffffff` | `#000000` |
| `--ink` (text, rules) | `#000000` | `#ffffff` |
| `--dim` | `#555555` | `#9a9a9a` |
| `--faint` | `#999999` | `#666666` |
| `--mute` | `#bbbbbb` | `#4a4a4a` |
| `--soft` | `#e6e6e6` | `#262626` |
| `--hover` | `#f4f4f4` | `#141414` |
| `--ok` | `#1f9d55` | `#3ecf7a` |
| `--alarm` | `#b3261e` | `#ff6b62` |

Mascot palette (coin art only, never UI): Pepe green, robe orange, royal blue ground, coin gold. IMD Radar adds mint `#7CF5C8` on `#05070a`.

## 4. Type

- Everything: **IBM Plex Mono** (OFL-1.1), fallback `ui-monospace, SFMono-Regular, Menlo, monospace`.
- Sizes are small and dense: labels 10–11 px with `0.06em` tracking, body 12–13 px, headings 18 and 28 px.
- IMD Radar's sister style: Geist, Geist Mono, Instrument Serif (all on Google Fonts).

## 5. Layout and components

- Rules are lines, not shadows: `1.5px solid var(--ink)`.
- Side gutter `clamp(16px, 4vw, 34px)`. Pill controls 40 px tall.
- Square corners. No gradients in the interface.
- Instruments: segmented bars (`--seg-mid`, `--seg-light`) and dials, as on the share card.
- Light and dark themes are both first-class (`data-theme="dark"`).

## 6. Voice

Terse, technical, lower case where the site uses it. Numbers before adjectives. The swarm is described by what it did, with a link to the record.

## 7. Provenance and rights

Every file here was copied on 2026-10-14 from IMD's public pages: imd.fun (icon, favicon, app icon, share card, walking Pepe, stylesheet tokens) and imdradar.site (coin logos, Radar logo and icon, font list); the 800 px coin logo is the image on IMD's DexScreener listing. The marks and art belong to IMD and to their artists. Pepe the Frog is Matt Furie's character. This package claims no ownership and grants no licence; it is a record of the current identity, offered so the community vote can confirm it as the base. Hashes of every file are in `MANIFEST.txt`.

## 8. Make your own

`template/visualidentity-template.md` is a fill-in copy of this guide for a new project in the IMD style: keep the tokens, type and rules, and start the mark from the family base, `assets/family-base-pepe.png`: IMD's coin Pepe in a light neutral palette, with a plain rim instead of IMD's gold star coin. Change its background, skin, outfit, eyes, hat or hair, moustache or accessory, or frame. The template includes the image-job request text. `example/family.html` shows the three side by side (IMD official, family base, an example project) with the two image jobs that drew them.
