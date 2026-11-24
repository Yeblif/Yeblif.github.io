# Yeblif.github.io
Index of my GitHub Pages sites.

## What it does
Serves https://yeblif.github.io/ as a contents page listing every public
Yeblif repo that has GitHub Pages enabled (forks excluded), with a link to
the live site, the repo, its description, topic tags and last-updated date.

A GitHub Action builds `repos.json` and deploys the site with it — daily,
on every push to `main`, and on demand. The page reads that file, so visitors
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
- `.github/workflows/update-repos.yml` — the Action that builds `repos.json`
  and deploys the site. `repos.json` exists only in the deployed site, not
  in the repo. Needs **Settings → Pages → Source: GitHub Actions**.
- `.nojekyll` — tells Pages to serve files as-is, without Jekyll.
- `CHANGELOG.md` — version history.
- `.github/` — issue and pull request templates.

## Changelog
See [CHANGELOG.md](CHANGELOG.md).
