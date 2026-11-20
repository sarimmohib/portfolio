# Sarim Mohib — portfolio

A single-file portfolio site. No build step, no dependencies, no framework.

## View it

Open `index.html` in a browser, or serve the folder locally:

```bash
cd /root/Projects/sarim-portfolio
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy

Copy `index.html` to any static host. For GitHub Pages:

1. Create a public repo (for example `sarimmohib.github.io`).
2. Commit `index.html` at the root.
3. Settings → Pages → Source: **Deploy from a branch** → `main` / `/`.
4. Your site appears at `https://sarimmohib.github.io/`.

Remote Google Fonts (Space Grotesk + IBM Plex Mono) load over HTTPS; the page falls back to system fonts offline.

## What's in it

- **Arcade CRT HUD** visual direction — charcoal neutral ramp, one amber accent, scanlines and corner brackets, no gradients, glows or emoji.
- **Motion does the "game" work:** a segmented scroll-progress rail, staggered scroll reveals, quiet hover transitions on cards and buttons, and a one-time scan sweep on the player card. `prefers-reduced-motion` is respected.
- **Responsive** layout with a collapsible mobile menu.
- **Public work only.** The quest log links exclusively to the two public repositories (`trinity`, `opencode-swarm-integration`) plus the public profile. No private repo names or links appear anywhere in the file.

## Editing

- Name, bio, stats and project copy: search the `<!-- HERO -->`, `<!-- ABOUT / LOADOUT -->` and `<!-- QUESTS / PROJECTS -->` sections.
- Colors and spacing: the `:root` custom properties at the top of the `<style>` block.
- To add email or social links, put them in the `<!-- CONTACT -->` section next to the GitHub button.

Design direction informed by [unslop](https://x.com/heydamir) by Damir Sokolovsky, CC BY 4.0.
