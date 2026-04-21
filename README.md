# nauder.dev

Personal portfolio site built with [Astro 6](https://astro.build), deployed to [GitHub Pages](https://pages.github.com) at [nauder.dev](https://nauder.dev).

## Stack

- **Astro 6** — static site generation, zero JS by default
- **Vanilla CSS** — CSS custom properties for design tokens, no framework
- **GitHub Actions** — automated build and deploy on every push to `main`
- **GitHub Pages** — free static hosting with custom domain

## Development

```sh
npm install       # install dependencies
npm run dev       # dev server at localhost:4321
npm run build     # build static site to ./dist/
npm run preview   # preview the production build locally
npx astro check   # type-check .astro files
```

Requires Node >= 22.12.0.

## Project structure

```
src/
├── components/        # Nav, Footer, ProjectCard
├── content/
│   └── projects/      # Markdown files — one per project
├── layouts/
│   └── BaseLayout.astro
├── pages/
│   ├── index.astro
│   ├── contact.astro
│   └── projects/[slug].astro
└── styles/
    └── global.css     # design tokens (colors, spacing, radius)
```

## Adding a project

Create a Markdown file in `src/content/projects/` with the following frontmatter:

```md
---
title: "My Project"
description: "Short description shown on the card."
tags: ["TypeScript", "React"]
github: "https://github.com/..."   # optional
demo: "https://..."                # optional
featured: true                     # optional — highlights the card
order: 1                           # optional — controls sort order
---

Project details go here...
```

## Deployment

Pushing to `main` triggers the GitHub Actions workflow (`.github/workflows/`), which runs `npm ci && npm run build` and deploys `./dist/` to GitHub Pages. The custom domain is configured via the `CNAME` file at the repo root.
