# ROBN Synth — brand notes

Derived from the ROBN logo artwork in `2 R O B N  Holdings LTD/02_DESIGN/01_Brand`
on the ROBN 3TB drive. There was no written guideline, so this records what the
UI uses and why. Treat it as a working draft, not the official ROBN guide.

## Logo

| Asset | Use |
|---|---|
| `assets/robn-wordmark.png` | Header wordmark. Cropped from *ROBN LOGO 2021*, 900px wide for 2x screens. |
| `assets/robn-mark.png` | The neon R button. Header badge. |
| `assets/favicon.png` | 64px R button. |

- Only ever put the logo on dark grounds (`#10001C` or darker). It's a neon glow
  and goes muddy on light backgrounds.
- The wordmark carries a grey halo in the source art; the CSS lifts it with
  `brightness(1.45)` plus a teal drop-shadow. Don't recolour the letters.
- Product name sits to the right of the wordmark in Cinzel, spaced caps, behind
  a thin teal divider: **ROBN | SYNTH**.

## Colour

Sampled from the artwork, not picked by eye.

| Token | Hex | From | Use |
|---|---|---|---|
| `--teal` | `#00F0D8` | wordmark glow | Primary accent, Layer A, active white keys |
| `--ice` | `#78D8F0` | button ring | Secondary headings, product name, focus rings |
| `--ember` | `#FF3B1F` | fire inside the R (lifted for legibility) | Accent, Layer B, Panic, active black keys |
| `--ember-deep` | `#D40000` | fire inside the R | Ember fills |
| `--bg` | `#10001C` | R background | Page ground |
| `--glass` | `#243048` @ 38% | button glass | Panels |

Teal is the default voice; ember is the spark. Keep ember to a few points per
screen or it stops reading as an accent.

## Type

- **Display:** Cinzel (Google Fonts, SIL OFL), uppercase, wide tracking.
  It stands in for Exodus, the wordmark face.
- **UI:** Inter (Google Fonts, SIL OFL).

**Exodus licence:** the copy on the drive is the *Personal Use* licence
(Andrew Herndon, 2015). It explicitly forbids including the font in a website
without written permission, so it is **not** embedded here. A commercial licence
is sold at https://gumroad.com/l/exodus. Once you have one, add the WOFF files
and swap `--display` to Exodus.
