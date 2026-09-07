# McNulty Capital Management — public site

Static marketing site for **McNulty Capital Management Pte. Ltd.** (Singapore UEN 202329748D): asset management and advisory focused on crypto options and volatility.

## Files

| File | Purpose |
|------|---------|
| `index.html` | Single-page site (hero through contact) |
| `styles.css` | Theme and layout |
| `privacy.html` / `terms.html` | Short legal stubs |
| `.nojekyll` | Disables Jekyll processing on GitHub Pages |

## Local preview

Open `index.html` in a browser, or from this folder:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080/`. Styles load via relative `styles.css`.

## GitHub Pages

Intended publish URL:

`https://seanbmcnulty.github.io/mcnultycapitalmanagement/`

This is a **project** site, so the base path is `/mcnultycapitalmanagement/`. All asset and in-site links use **relative paths** (e.g. `styles.css`, `privacy.html`, `#contact`) so they resolve correctly both locally and under that prefix.

Typical setup:

1. Push this folder’s contents to the `gh-pages` branch (or the branch/folder configured for Pages) of the `mcnultycapitalmanagement` repository.
2. In repo **Settings → Pages**, serve from that branch’s root (or `/docs` if you place these files there).
3. `.nojekyll` ensures underscored paths and raw static assets are not filtered by Jekyll.

No build step is required.
