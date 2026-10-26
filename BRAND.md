# ROBN Synth — brand notes

**Source of truth:** `robn-theme.css`, copied unedited from the ROBN brand
handoff (`~/Claude/Projects/ROBN Site/robn-handoff/`). Build against its
tokens; never hardcode a hex that already exists as a token. To update the
brand, replace that file with a newer handoff copy rather than editing it here.

## How the synth maps to the tokens

| Surface | Token |
|---|---|
| Page backdrop, scope background | `--void` |
| Panels, header | `--ground` |
| Inputs, list hover | `--raised` / `--raised-2` |
| Borders / dividers, slider tracks | `--line` / `--line-soft` |
| Layer A, active white keys, selected patch, primary actions | `--accent` (mint) + `--glow-mint` |
| Layer B, active black keys, focus rings | `--accent-cyan` + `--glow-cyan` |
| Panic | `--danger` |
| Warning note (Omnisphere notice) | `--warning` |
| Text | `--fg-1` primary, `--fg-2` secondary, `--fg-3` labels/meta |

Glow is reserved for active or interactive state: a slider you're touching, a
pressed key, a focused control. Everything at rest is flat.

## Type

- **IBM Plex Mono** (`--font-mono`) for all UI chrome: panel headers, labels,
  buttons, values, patch list.
- **Cinzel** (`--font-display`) only for brand moments: the **SYNTH** product
  label and the current patch title.
- Cinzel stands in for ROBN's display face **Exodus**. The copy on the drive is
  a *Personal Use* licence that forbids web embedding; a commercial licence is
  at https://gumroad.com/l/exodus. Once licensed, swap `--font-display` in a
  newer `robn-theme.css`.

## Logos

All from `robn-handoff/logos/`, cropped and resized for the web.

| Asset | Source | Use |
|---|---|---|
| `assets/robn-r-chrome.png` | `robn-r-chrome.png` | App icon, 40px, header left |
| `assets/robn-wordmark.png` | `robn-wordmark.png` | Header wordmark, 26px tall, mint drop-shadow per handoff |
| `assets/favicon.png` | `robn-r-outline.png` | Favicon, on `--void` so it reads in light browser chrome |
