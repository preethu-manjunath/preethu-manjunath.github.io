# preethu-manjunath.github.io

Personal site of Preethu Nath Manjunath — **[preethu-manjunath.github.io](https://preethu-manjunath.github.io/)**

```
index.html                    one screen: name, links, avatar over real energy footage (Mixkit)
resume.html                   short text résumé with an interactive knowledge-graph diagram
assets/preethu.jpg            portrait
.github/workflows/deploy.yml  publishes to GitHub Pages on every push to main
```

No build step. Both pages are single HTML files. Background clips stream from
Mixkit's CDN (free licence); the next clip only loads while the current one plays.

## Editing content

- **Background clips:** the `CLIPS` list of Mixkit video IDs in `index.html`.
- **Résumé:** plain HTML in `resume.html`.

## Running locally

```bash
python3 -m http.server 8000
```

## Deploying

Push to `main`. Pages must be set to **Settings → Pages → Source: GitHub Actions**.
