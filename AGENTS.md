# AGENTS.md — calculadorasofipos-web

## What this is

A single-page static HTML site for the "Calculadora SOFIPOS México" Android app, deployed via GitHub Pages.

## Quick facts

- **No build step.** `index.html` is the only page — plain HTML + inline CSS. No framework, bundler, or dependencies.
- **GitHub Pages** deploys from the `main` branch. Custom domain (`calculadorasofipos.com`) is configured via the root `CNAME` file — keep it present.
- **SEO files** include `robots.txt`, `sitemap.xml` (single URL entry).
- **Favicons** live in `images/` (`icon.ico`, `icon.png`).
- **Language:** Spanish (`lang="es"`). All visible text is in Spanish.
- **No tests, linting, formatting, typechecking, or CI** — none are configured.
- **Android app** is published on Google Play: `com.thisisthetime.calculadorasofipos`.

## Commands

None. There is no dev server, build, or test command. For local preview, serve the directory with any static file server:

```sh
npx serve .
# or: python3 -m http.server
# or: live-server .
```

## Editing conventions

- All CSS is embedded in `<style>` inside `index.html` — no external stylesheets.
- Keep inline CSS in the `<head>` block, not as element-level `style` attributes.
- External image URLs point to Google Play CDN screenshots — do not commit those images locally.
- Footer links: developer site (`programmingheadache.com`), privacy policy link.
