# Sunzal Digital website

The portfolio site for Sunzal Digital: who I am, what I do, and the websites I've built.

It's plain HTML and CSS with no build step. Everything the site serves lives in `public/`:

- `public/index.html` — the page content
- `public/style.css` — styles
- `public/images/` — screenshots of client sites

## Preview locally

Open `public/index.html` in a browser, or run `npx http-server public`.

## Deploy (Cloudflare)

```sh
npx wrangler deploy
```

## Adding a new project

Copy one of the `<article class="project">` blocks in `public/index.html`, update the text and link,
and add a 1440×900 screenshot of the site to `public/images/`.
