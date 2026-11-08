# Vortexweb

Landing page for [vortexweb.ch](https://vortexweb.ch): a single page with an interactive particle vortex in the background and a contact card.

## Structure

- `index.html` — the whole site: markup, styles and the canvas animation script
- `images/` — logo and favicon
- `CNAME` — custom domain for GitHub Pages

There is no build step and no dependencies apart from the Outfit font from Google Fonts.

## Run locally

Open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Deploy

The site is hosted on GitHub Pages. Pushing to `main` publishes it.

## Editing

- Text and contact email: in the `<body>` of `index.html` (the email also appears in the copy-button script)
- Colors: CSS variables in `:root` at the top of the `<style>` block
- Animation: `PARTICLE_COUNT`, `colorPalette` and `ARM_COUNT` in the script at the bottom
