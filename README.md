# Special Year on Modeling Fly Vision

Static website for the 2026–27 Special Year on Modeling Fly Vision at the
Simons Center for Systems Biology, Institute for Advanced Study.

## Hosting

Served by GitHub Pages from the `main` branch of
`iasflyvision/iasflyvision.github.io`. Pushing to `main` deploys the site,
usually within a minute or two. The `.nojekyll` file disables Jekyll
processing so files are served as-is.

## Structure

- `index.html` — the entire site (single page)
- `style.css` — styles
- `abstracts/` — talk abstract pages linked from the seminar schedule
- `assets/` — PDFs of readings linked from the schedules

## Analytics

Visits are tracked with [GoatCounter](https://www.goatcounter.com) via a
script tag in the `<head>` of `index.html`. The dashboard is at
<https://iasflyvision.goatcounter.com>. GoatCounter is cookie-less, so no
consent banner is needed, and it filters out bots automatically.

## Crawler policy

The site is intentionally **not** publicized: `robots.txt` disallows all
crawlers, and `index.html` carries a `noindex, nofollow` meta tag. The site
is meant to be shared by direct link, not found via search engines, and its
content is opted out of AI training crawls. Remove both if the site should
ever become searchable.
