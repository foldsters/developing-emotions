# emotions.dev

A one-page lexicon for the feelings only developers feel.

Part of why developers burn out is that we go through things we have no language
for — so we can't name them, can't share them, and end up carrying them alone.
This is a small, growing dictionary of coined words for those emotions. The
aesthetic: flowers blooming up through cold brutalist concrete.

## Stack

- [Astro](https://astro.build) — static one-page site (`src/pages/index.astro`)
- Deployed to GitHub Pages via `.github/workflows/deploy.yml`
- Served from the custom apex domain **emotions.dev** (`public/CNAME`)

## Develop

```sh
npm install
npm run dev      # local dev server at http://localhost:4321
npm run build    # production build to ./dist/
npm run preview  # preview the production build
```

## Deploy

Pushing to `main` triggers the GitHub Actions workflow, which builds the site and
publishes it to GitHub Pages. The `public/CNAME` file keeps the custom domain
bound on every deploy.
