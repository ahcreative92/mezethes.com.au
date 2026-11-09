# Mezethes Greek Taverna website

Static copy of the site formerly hosted on Webflow (mezethes-website.webflow.io), self-contained for hosting on Vercel.

- `index.html` – home (`/`)
- `mezethes-menu.html` – `/mezethes-menu`
- `mezethes-wine-list.html` – `/mezethes-wine-list`
- `css/`, `js/`, `images/`, `files/` – all assets (Webflow interactions run from the local `js/` files)

`vercel.json` enables clean URLs so `/mezethes-menu` serves `mezethes-menu.html`. No build step: on Vercel choose Framework "Other", leave build command empty, output directory `.`.

Preview locally: `python3 -m http.server 8000` then open http://localhost:8000 (clean URLs only work on Vercel; locally use `/mezethes-menu.html`).

## Deployment

Repo: https://github.com/ahcreative92/mezethes.com.au — connected to the Vercel project `mezethes-website`. Every push to `main` deploys to production (https://mezethes-website.vercel.app).
