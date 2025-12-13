# Ryan Wang — Personal Website (Clean Jekyll / GitHub Pages)

This repo is a lightweight, low-maintenance personal website built with **Jekyll** + **Minimal Mistakes** via `remote_theme`,
so you don't need to vendor a giant theme repo.

## Deploy on GitHub Pages
1. Create (or reuse) a repo named **ryanwang1203.github.io**.
2. Put these files at the repo root.
3. Go to **Settings → Pages**:
   - Source: **Deploy from a branch**
   - Branch: **main** / **root**
4. Save. Your site should build automatically.

## Where to edit content
- Home: `index.md`
- News list: `news.md` + posts in `_posts/`
- Papers list: `papers.md` + items in `_publications/`
- Projects list: `projects.md` + items in `_projects/`
- Experience: `experience.md`

## Add a new project
Create a file in `_projects/` like `my-project.md` with front matter + content.

## Add a new paper
Create a file in `_publications/` like `paper-2021-jd-logistics.md`.

## Optional: local preview
If you want local preview, install Ruby + Bundler and run:
```bash
bundle install
bundle exec jekyll serve
```
