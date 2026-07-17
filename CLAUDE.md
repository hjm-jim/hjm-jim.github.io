# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a minimal Jekyll-based GitHub Pages personal website for Jingming Hu (胡景明), hosted at `hjm-jim.github.io`. All content lives in a single `index.md` file with three sections: personal info, project details, and blog post links.

## Commands

```bash
# Install dependencies
bundle install

# Run development server (http://localhost:4000)
bundle exec jekyll serve -l -H localhost

# Build for production
bundle exec jekyll build
```

## Architecture

The site is deliberately minimal — only 5 core files:

| File | Purpose |
|---|---|
| `_config.yml` | Jekyll config: site metadata, author info (rendered in sidebar), markdown settings |
| `_layouts/default.html` | Single HTML layout: sticky header nav, sidebar (avatar/bio/links), main content, footer |
| `index.md` | **The only content file** — all text and images go here. Three sections: about, projects, posts |
| `assets/css/style.css` | All styling: CSS variables with dark mode, responsive grid, card components |
| `Gemfile` | Minimal: `github-pages` + `webrick` gems |

### How to edit

- **Edit content**: Open `index.md`, write Markdown. Use the provided HTML snippets for project cards (`<div class="project-grid">`) and post links (`<div class="post-list">`).
- **Edit author info**: Update the `author` block in `_config.yml` (name, avatar, bio, location, email, github).
- **Edit styling**: Modify `assets/css/style.css`. CSS variables in `:root` control colors; `@media (prefers-color-scheme: dark)` overrides for dark mode.
- **Add images**: Place files in `images/`, reference as `![alt](/images/filename.png)`.
- **Add pages**: Create new `.md` files at root level with `layout: default` frontmatter.

### Design conventions

- No JavaScript — pure HTML + CSS
- System dark/light mode via `prefers-color-scheme` media query
- Responsive: two-column (sidebar + content) on desktop, single-column on mobile
- Max content width 960px
- Chinese-friendly typography (PingFang SC, Microsoft YaHei font stack)
