# driftnotes

A personal blog for travel, experiences, and academic writing — built with
Jekyll, styled after Gregory Gundersen's minimal blog theme
(https://github.com/gwgundersen/blog-theme).

## Setup

1. Install Ruby + Bundler if you don't have them already.
2. Install dependencies:
   ```bash
   bundle install
   ```
3. Preview locally:
   ```bash
   bundle exec jekyll serve
   ```
   Visit http://localhost:4000

## Publishing to GitHub Pages

1. Push this repo to `https://github.com/driftnotes/driftnotes.github.io`
   (repo name must be exactly `driftnotes.github.io`).
2. In the repo, go to **Settings → Pages** and confirm the source is set to
   the `main` branch (GitHub Pages auto-builds Jekyll sites — no extra config
   needed).
3. Site goes live at `https://driftnotes.github.io` within a minute or two.

## Writing a new post

Add a new file to `_posts/` named `YYYY-MM-DD-title.md`:

```markdown
---
title: Your Post Title
subtitle: A one-line subtitle/description.
date: YYYY-MM-DD
categories: travel   # or: academic / personal
published: true
---

Your content here, in Markdown.
```

Categories currently supported: `travel`, `academic`, `personal`. Each has
its own listing page (`/travel/`, `/academic/`, `/personal/`), and the
homepage lists everything together, newest first.

## Math (for academic posts)

KaTeX is enabled. Inline math: `$x^2$`. Block math:
```
$$
\int_0^1 x^2 \, dx = \frac{1}{3}
$$
```

## Structure

```
_config.yml       site settings (title, description, plugins)
_layouts/         page templates
_includes/        shared snippets (nav bar)
_posts/           your posts live here
css/              theme styling
travel/           travel category page
academic/         academic category page
personal/         personal category page
index.html        homepage (lists all posts)
```

## Customizing

- Edit `_config.yml` to change the site title, description, or your name.
- Edit `css/blog.css` to change colors, fonts, spacing.
- Edit `index.html` to change the homepage quote/intro.
