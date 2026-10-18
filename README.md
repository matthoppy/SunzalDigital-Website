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

1. Copy one of the `<article class="case">` blocks in the Work section of `public/index.html`, give it a new `id`,
   and update the name, place, link, summary and "What I did" list. The `case-a`, `case-b` and `case-c` classes
   set the layout: large image left, large image right, or one full-width image with three below.
2. Add screenshots to `public/images/` as WebP:
   - desktop views: 1440×900 viewport at 1.5× (2160×1350)
   - phone view for the hero row: 390×844 viewport at 2× (780×1688), named `name-mobile.webp`
3. To show the new site in the hero, add it to `.horizon-sites` and `.horizon-captions`.

## Brand

Colours, type and logo files live in `public/brand/`, with a guide page at `/brand/`.
The type is Archivo (Semi Expanded for headings, normal width for text) from Google Fonts.
