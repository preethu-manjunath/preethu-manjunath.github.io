# preethu-manjunath.github.io

Personal site of Preethu Nath Manjunath — **[preethu-manjunath.github.io](https://preethu-manjunath.github.io/)**

```
index.html                    realistic 3D landscape (three.js + Poly Haven CC0 sky, textures, plants)
resume.html                   short text résumé with an interactive knowledge-graph diagram
assets/preethu.jpg            portrait
.github/workflows/deploy.yml  publishes to GitHub Pages on every push to main
```

No build step. Both pages are single HTML files. The 3D page loads three.js from
jsDelivr and CC0 assets straight from Poly Haven's CDN (~20 MB on first visit).

## Editing content

- **3D scenes:** the `SCENES` (text) and `SHOTS` (camera) arrays in `index.html`.
- **Résumé:** plain HTML in `resume.html`.

## Running locally

```bash
python3 -m http.server 8000
```

## Deploying

Push to `main`. Pages must be set to **Settings → Pages → Source: GitHub Actions**.
