# theme_template

Starting point for a DimOS dashboard app. Copy this folder and build on it.

- `theme.css` — the retro-futuristic design system: tokens (`--neon`, surfaces,
  `--display`/`--pixel`/`--mono`) + components (`.dim-btn`, `.dim-card`, `.dim-input`,
  `.dim-tabs`, `.dim-table`, calendar, stepper, charts, …). Reskin by overriding the
  `:root` tokens.
- `fonts.css` — base64-embedded fonts: PixelOS (logo/captions), DisplayOS /
  Chakra Petch (headings), RetroMono / JetBrains Mono (body).
- `index.html` — a living styleguide showing every component. Open it directly in a
  browser, or browse the binary-served copy at `/theme`.
- `main.js` — app entry stub (`init` / `uiResponse` / `backendResponse`).

When served by the `dim` binary, link the shared copies instead of bundling your own:
`/assets/theme.css` and `/assets/fonts.css`.
