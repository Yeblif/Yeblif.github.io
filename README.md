# Yeblif.github.io
Index of my GitHub Pages sites.

## What it does
Serves https://yeblif.github.io/ as a contents page listing every public
Yeblif repo that has GitHub Pages enabled (forks excluded), with a link to
the live site, the repo, its description, topic tags and last-updated date.

The list lives in `repos.json`, which a GitHub Action rebuilds daily, on
every push to `main`, and on demand. The page reads that file, so visitors
never hit GitHub's API rate limit (60 requests/hour per IP, shared by
everyone on a work network). New Pages sites appear automatically — no
edits needed here.

## How to use
- Visit https://yeblif.github.io/.
- Search by name/description, or filter by topic tag (work, c3d, homelab,
  fusion, …).
- To make a repo's card look good: fill in its **About** description and
  topics on GitHub.
- New site not showing yet? Press **↻ Refresh** to check GitHub live, or
  run **Actions → Update repo list → Run workflow** to update `repos.json`
  straight away. If the live check is rate-limited, the page keeps showing
  the last saved list.

## Files
- `index.html` — the whole page (HTML, CSS and JS in one file).
- `repos.json` — the generated list of Pages sites (don't edit by hand).
- `.github/workflows/update-repos.yml` — the daily Action that builds `repos.json`.
- `.nojekyll` — tells Pages to serve files as-is, without Jekyll.
- `CHANGELOG.md` — version history.
- `.github/` — issue and pull request templates.

## Changelog
See [CHANGELOG.md](CHANGELOG.md).
