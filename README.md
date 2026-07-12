# Rusty the Raccoon is Scared of the Dark

Static Astro rebuild of [rustytheraccoon.com](https://www.rustytheraccoon.com), the site for
Michelle Trotta's children's book *Rusty the Raccoon is Scared of the Dark*. The original Wix
site is being retired; this project reproduces its content and structure with a cleaner, faster,
self-hosted build. Deploys to Cloudflare Pages.

The full scrape of the original site (HTML, images, PDFs, and a content manifest) lives in
`scrape/` for reference and is not part of the build.

## Project Structure

```text
/
├── public/
│   ├── activities/       # 11 downloadable activity PDFs
│   ├── _redirects        # Cloudflare Pages redirect rules
│   └── robots.txt
├── src/
│   ├── assets/images/    # Optimized images (astro:assets)
│   ├── components/       # Header, Footer
│   ├── layouts/          # BaseLayout (SEO meta, fonts, header/footer)
│   ├── pages/             # index, about, author, activities, resources, videos, contact
│   └── styles/global.css # Design tokens, fonts, shared component styles
└── scrape/               # Archived original site content (reference only, untouched)
```

## Commands

| Command           | Action                                       |
| :----------------- | :-------------------------------------------- |
| `npm install`       | Install dependencies                          |
| `npm run dev`       | Start local dev server at `localhost:4321`    |
| `npm run build`     | Build the production site to `./dist/`        |
| `npm run preview`   | Preview the production build locally          |

## Design

- **Deep teal** `#144c53` — sampled from the original site's section background color.
- **Cream** `#f7f3ea` — sampled from the original site's decorative background art.
- **Amber** `#f2a93b` / **coral** `#ef6f63` — accent colors echoing the book's own artwork,
  including the glowing jar of fireflies that Rusty and Squeaks carry through the dark — the
  site's recurring "firefly-glow" signature motif.
- **Fredoka** (display) + **Nunito Sans** (body), self-hosted via `@fontsource`.
