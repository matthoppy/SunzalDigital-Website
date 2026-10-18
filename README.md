# Sunzal Digital website

The portfolio site for Sunzal Digital: who I am, what I do, and the websites I've built.

It's plain HTML and CSS with no build step. Everything the site serves lives in `public/`:

- `public/index.html` — the page content
- `public/style.css` — styles and brand tokens (colours, type, spacing)
- `public/images/` — screenshots of client sites
- `public/brand/` — logo files (SVG and PNG), social share image and the brand guide (`/brand/`)

## Preview locally

Open `public/index.html` in a browser, or run `npx http-server public`.

## Deploy

**GitHub Pages:** every push to `main` publishes `public/` via `.github/workflows/pages.yml`.
In the repo's Settings → Pages, set **Source** to **GitHub Actions** (one-time).

**Cloudflare (alternative):**

```sh
npx wrangler deploy
```

## Adding a new project

Copy one of the `<article class="case">` blocks in `public/index.html`, update the number, text, links and
`--tint` panel colour, then add two screenshots to `public/images/`:

- `name.jpg`: desktop, 1440×900 viewport at 1.5× (2160×1350)
- `name-mobile.jpg`: phone, 390×844 viewport at 2× (780×1688)
