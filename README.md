# LSaiko — Portfolio Landing Page

A single-file, dependency-free landing page showcasing all public projects across
medical imaging AI, FDA/ISO regulatory tooling, and public-health data products.

Live repository data (repo count, stars, primary language, per-project stars/forks
and last-updated time) is fetched at runtime from the GitHub REST API, with a 30-minute
`localStorage` cache and a graceful fallback to the static figures baked into the page.

## Deployment

Deployed via GitHub Pages using the workflow in `.github/workflows/deploy.yml`
(builds on every push to `main`). No build step — `index.html` is served as-is.

## Local preview

Just open `index.html` in a browser, or serve the folder:

```bash
python -m http.server 8000
```
