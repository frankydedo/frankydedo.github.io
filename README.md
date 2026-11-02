# frankydedo.github.io

Personal portfolio of **Francesco Pio De Dominicis** — Generative AI engineer, MSc in Computer Engineering (AI & Data Analysis) at Politecnico di Torino.

**Live:** https://frankydedo.github.io · Italian version: https://frankydedo.github.io/it/

## Stack

Plain HTML + CSS. No framework, no build step, no JavaScript. Hosted on GitHub Pages from the `main` branch.

- The theme follows the OS (`prefers-color-scheme`), light and dark.
- Fonts: SF Pro on Apple devices via the system stack, Inter elsewhere (Google Fonts), JetBrains Mono for labels.

## Structure

```
.
├── index.html                          # English (default)
├── it/index.html                       # Italian
├── assets/
│   ├── css/style.css                   # design tokens, Liquid Glass, components, responsive rules
│   ├── Francesco-Pio-De-Dominicis-CV.pdf
│   └── favicon.svg
└── .nojekyll                           # serve files as-is on GitHub Pages
```

## Design

Design system **"Pro Glass"**: a monochrome canvas (black / `#F5F5F7`), monumental type, a warm gradient on headlines, and Liquid Glass on foreground containers only (nav capsule, cards, timeline, CTA).

The `.glass` component in `style.css` combines translucent fill, `backdrop-filter: blur() saturate()`, a 1px specular rim drawn with a CSS mask, and an inset top highlight.

## Run locally

```bash
python3 -m http.server 4321
```

Then open http://localhost:4321.

## Update and deploy

1. Edit the content in **both** `index.html` and `it/index.html`.
2. Check it locally.
3. Commit and push to `main`. GitHub Pages republishes in about a minute.

```bash
git commit -am "Update experience" && git push
```

To update the CV, replace `assets/Francesco-Pio-De-Dominicis-CV.pdf` and keep the same file name.
