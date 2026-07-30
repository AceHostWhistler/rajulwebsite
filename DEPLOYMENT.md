# Deployment Instructions

This site deploys automatically to GitHub Pages when changes are pushed to `main`.

## Enable GitHub Pages

1. Go to repository **Settings → Pages**
2. Under **Build and deployment**, set **Source** to **GitHub Actions**
3. After the next push to `main`, the workflow publishes the built site from the `dist/` folder

## Custom domain (recommended)

To serve the site on its own domain instead of a GitHub-hosted URL:

1. Purchase or use a domain you control (e.g. `pickleballcoachseattle.com`)
2. In **Settings → Pages → Custom domain**, enter your domain
3. Add the DNS records GitHub provides (usually `A` records and a `CNAME` for `www`)
4. Enable **Enforce HTTPS**

Using a custom domain keeps this site fully independent in search results and branding.

## Local development

```bash
npm install
npm run dev
```

## Manual build

```bash
npm run build
```

The static site output is written to `dist/`.
