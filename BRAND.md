# ROBN Synth — brand notes

Derived from the ROBN logo artwork in `2 R O B N  Holdings LTD/02_DESIGN/01_Brand`
on the ROBN 3TB drive. There was no written guideline, so this records what the
UI uses and why. Treat it as a working draft, not the official ROBN guide.

## Logo

| Asset | Use |
|---|---|
| `assets/robn-wordmark.png` | Header wordmark. Cropped from *ROBN LOGO 2021*, 900px wide for 2x screens. |
| `assets/robn-mark.png` | The heat-map R (*New R Logo (Final)*), transparent cut-out. Header mark at 56px, free-floating with a teal + ember drop-shadow that follows the letter. |
| `assets/favicon.png` | 64px heat-map R on violet-black `#10001C`, so the dark-bodied letter reads in a browser tab. |

- Only ever put the logo on dark grounds (`#10001C` or darker). It's a neon glow
  and goes muddy on light backgrounds.
- The wordmark carries a grey halo in the source art; the CSS lifts it with
  `brightness(1.45)` plus a teal drop-shadow. Don't recolour the letters.
- Product name sits to the right of the wordmark in Cinzel, spaced caps, behind
  a thin teal divider: **ROBN | SYNTH**.
- Use the transparent heat-map R, not the boxed square version, so the mark
  floats on the page rather than reading as a pasted-on tile.

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

- **Everything:** IBM Plex Mono (Google Fonts, SIL OFL), weights 400–700.
  Headings in uppercase with 0.18–0.2em tracking; mono is already wide, so
  keep tracking tighter than you would on a proportional face.
- Fallbacks: `ui-monospace, "SF Mono", Menlo, monospace`.

**Exodus licence:** the copy on the drive is the *Personal Use* licence
(Andrew Herndon, 2015). It explicitly forbids including the font in a website
without written permission, so it is **not** embedded here. A commercial licence
is sold at https://gumroad.com/l/exodus. Once you have one, add the WOFF files
and use it for the wordmark or display headings (`--display`).
