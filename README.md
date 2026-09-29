# preethu-manjunath.github.io

Personal site of Preethu Nath Manjunath — **[preethu-manjunath.github.io](https://preethu-manjunath.github.io/)**

```
index.html                    "Power × Intelligence" — a small 3D energy world (three.js)
resume.html                   the plain résumé, with an in-browser GraphRAG search console
assets/preethu.jpg            portrait
.github/workflows/deploy.yml  publishes to GitHub Pages on every push to main
```

No build step. Both pages are single HTML files; the only network requests are
Google Fonts, three.js from jsDelivr (world), and — only once a visitor asks the
résumé a question — transformers.js plus the MiniLM model (~23 MB, cached after).

## Editing content

- **World stops:** the `ZONES` array at the top of the script in `index.html`.
- **Résumé:** the HTML in `resume.html`, and the `CHUNKS` / `NODES` arrays that
  feed its search console (keep them in step with the visible text).

## Running locally

```bash
python3 -m http.server 8000
```

## Deploying

Push to `main`. Pages must be set to **Settings → Pages → Source: GitHub Actions**.
