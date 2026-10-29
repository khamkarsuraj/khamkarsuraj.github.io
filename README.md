# khamkarsuraj.github.io

Personal website of Suraj Khamkar, built with [Jekyll](https://jekyllrb.com/) on a trimmed-down
[al-folio](https://github.com/alshedivat/al-folio) theme.

## Pages

- `/` — about (`_pages/about.md`)
- `/projects/` — project cards from `_projects/`
- `/cv/` — rendered from `assets/json/resume.json`; PDF in `assets/pdf/`
- `/blog/` — posts from `_posts/` (not linked in the nav)

## Local build

```bash
bundle install
bundle exec jekyll serve
```

Or with Docker: `docker compose up` (see `docker-compose.yml`).

## Deploy

Pushes to `main` are built and published to the `gh-pages` branch by
`.github/workflows/deploy.yml`.
