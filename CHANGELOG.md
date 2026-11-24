# Changelog

All notable changes to this project are documented here.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]
### Added
- Self-updating contents page (`index.html`) listing every public repo with GitHub Pages enabled, with search and topic filters.
- Repo scaffold: README, CHANGELOG, issue/PR templates, `.nojekyll`.
### Changed
- Repo list cache cut from 1 hour to 5 minutes, with a Refresh button to fetch the latest list straight away.
### Fixed
- "GitHub API rate limit hit" on shared networks (e.g. work): the list now comes from `repos.json`, rebuilt daily by a GitHub Action (also on every push to `main`, or on demand from the Actions tab), so normal page loads never call the API. Refresh still checks live and falls back to the saved list instead of showing an error.
