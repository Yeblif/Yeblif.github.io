# Yeblif.github.io
Index of my GitHub Pages sites.

## What it does
Serves https://yeblif.github.io/ as a contents page. On load it asks the
GitHub API for Yeblif's public repos and lists every one that has GitHub
Pages enabled (forks excluded), with a link to the live site, the repo,
its description, topic tags and last-updated date. New Pages sites appear
automatically — no edits needed here.

## How to use
- Visit https://yeblif.github.io/.
- Search by name/description, or filter by topic tag (work, c3d, homelab,
  fusion, …).
- To make a repo's card look good: fill in its **About** description and
  topics on GitHub.
- Results are cached in the browser for an hour to stay inside the
  unauthenticated API limit (60 requests/hour per visitor).

## Files
- `index.html` — the whole page (HTML, CSS and JS in one file).
- `.nojekyll` — tells Pages to serve files as-is, without Jekyll.
- `CHANGELOG.md` — version history.
- `.github/` — issue and pull request templates.

## Changelog
See [CHANGELOG.md](CHANGELOG.md).
