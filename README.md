# Dimos Themes

A small collection of drop-in design systems for DimOS dashboard apps. Every theme exposes
the **same component API** (the `dim-*` classes — buttons, badges, form controls, stat cards,
progress bars, stepper, calendar, line/bar charts, tabs, data tables, alerts, avatars), so an
app can swap one stylesheet and keep all of its markup.

Each theme lives in its own folder under [`themes/`](themes/) with a self-contained
`index.html` styleguide you can open directly in a browser.

---

## 🕹 Retro Zero

Retro-futuristic HUD — neon-cyan hairlines, solid dark panels, faint scanlines, hard corners,
uppercase pixel/mono type, soft glow.

![Retro Zero — palette & typography](themes/retro_zero/screenshots/hero.png)

```html
<link rel="stylesheet" href="themes/retro_zero/fonts.css" />
<link rel="stylesheet" href="themes/retro_zero/theme.css" />
<body class="dimos"> ... </body>
```

<details><summary>Full styleguide</summary>

![Retro Zero — full styleguide](themes/retro_zero/screenshots/full.png)

</details>

---

## ☕ Caffeine

Warm, rounded, friendly — a faithful port of the
[Caffeine theme from tweakcn](https://tweakcn.com/editor/theme) (coffee/cream neutrals, soft
shadows, `0.5rem` corners) with a little extra accent flare so it isn't all brown (dusty teal,
warm sage, amber, muted plum).

![Caffeine — palette & typography](themes/caffeine/screenshots/hero.png)

```html
<link rel="stylesheet" href="themes/caffeine/theme.css" />
<body class="caffeine"> ... </body>
```

<details><summary>Full styleguide</summary>

![Caffeine — full styleguide](themes/caffeine/screenshots/full.png)

</details>

---

## 🔬 Science

A professional high-tech lab system: **mostly-white, clinical light mode** with a faint
precision grid, and a **high-class charcoal dark mode** with luminous instrument-blue accents.
Toggle modes with the button in the preview (or load with `#dark`).

| Light | Dark |
| --- | --- |
| ![Science — light](themes/science/screenshots/light.png) | ![Science — dark](themes/science/screenshots/dark.png) |

```html
<link rel="stylesheet" href="themes/science/theme.css" />
<body class="science"> ... </body>          <!-- light (default) -->
<body class="science dark"> ... </body>      <!-- high-class dark -->
```

---

## Reskinning

Every theme's colors are CSS variables at the top of its `theme.css` — override them to
retune a theme without touching components. The retro theme uses hex tokens (`--neon`,
`--accent-2`, `--bg`, …); Caffeine and Science use `oklch()` design tokens
(`--primary`, `--secondary`, `--info`, `--bg`, …), with Science's dark mode defined as
overrides on `body.science.dark`.
