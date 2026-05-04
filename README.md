# Portfolio

Personal portfolio site built with [Astro](https://astro.build) and deployed to GitHub Pages.

**Live:** [deka27.github.io/portfolio](https://deka27.github.io/portfolio/)

## Stack

- Astro 6, vanilla CSS, Inter (Google Fonts)
- Lucide icons (inline SVG)
- Light/dark theme with manual toggle (light by default)
- GitHub Actions for deploys

Built with minimal dependencies — just Astro and a touch of vanilla JavaScript for theme switching and scroll animations.

## Structure

```
.github/workflows/deploy.yml   build + deploy on push to main
public/                        static assets (favicon)
src/
  assets/                      images processed by Astro (hero.png), CV source
  layouts/Layout.astro         HTML shell, theme variables, global styles
  pages/index.astro            single-page portfolio
astro.config.mjs               site URL + base path
```

## Develop

```bash
npm install
npm run dev      # http://localhost:4321/portfolio/
npm run build    # production build to ./dist
npm run preview  # serve the built site locally
```

## Deploy

Pushes to `main` auto-deploy via [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml).

One-time setup: `Settings → Pages → Source: GitHub Actions`.

## Forking

Update [`astro.config.mjs`](astro.config.mjs) for your URL:

```js
export default defineConfig({
  site: 'https://<your-username>.github.io',
  base: '/<your-repo-name>',  // or '/' for a user/org page
});
```
