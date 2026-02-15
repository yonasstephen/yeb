# yonasstephen.com

Personal portfolio website built with [Astro](https://astro.build).

## Development

```bash
nvm use 18
npm install
npm run dev
```

## Build

```bash
npm run build
npm run preview
```

## Deployment

Deployed to GitHub Pages via GitHub Actions on push to `main`.

To set up:

1. Push this repo to GitHub
2. Go to repo Settings > Pages > Source > select "GitHub Actions"
3. Configure DNS: point `yonasstephen.com` to GitHub Pages ([docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site))

## Project Structure

```
content/
  about/          # About page markdown
  blog/           # Blog posts
  projects/       # Project pages
src/
  components/     # Nav, Footer, ProjectCard
  layouts/        # BaseLayout, MarkdownLayout
  pages/          # Route pages
  styles/         # global.css (design tokens)
public/           # Static assets, favicon, CNAME
```

## Adding Content

Add markdown files to `content/blog/` or `content/projects/` with the appropriate frontmatter:

**Blog post:**
```yaml
---
title: "Post Title"
description: "Short description"
date: 2024-01-01
tags: [tag1, tag2]
draft: false
---
```

**Project:**
```yaml
---
title: "Project Name"
description: "Short description"
tags: [tag1, tag2]
url: https://github.com/...
featured: true
date: 2024-01-01
---
```
