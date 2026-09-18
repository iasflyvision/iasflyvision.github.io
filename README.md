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

## Conventions

- **Readings** are listed below the topic in a schedule row, in author-year
  format ("Chung et al. (2021)"), separated by semicolons. Link to the DOI
  when one exists; otherwise to a PDF in `assets/` (URL-encode spaces in
  filenames) or an arXiv page.
- **Seminar rooms**: the intro line states the default (Dilworth Room);
  exceptions get a `<span class="venue">` note under the topic in their row.
- **Schedule layout**: column widths are controlled by the `.schedule` rules
  in `style.css` (date column, and the seminar table's topic column via
  `#seminars .schedule td:nth-child(2)`). No manual line breaks in titles.
- **Abstract pages** live in `abstracts/`, reuse the site header and
  stylesheet, and link back to the main page.
- **Local-only files**: the workshop flyer PDF in the repo root is untracked
  via `.gitignore`. Reading PDFs in `assets/` are committed and public.
- **Dates** use the "Sept. 4" style, consistent across both schedules.

## Crawler policy

The site is intentionally **not** publicized: `robots.txt` disallows all
crawlers, and `index.html` carries a `noindex, nofollow` meta tag. The site
is meant to be shared by direct link, not found via search engines, and its
content is opted out of AI training crawls. Remove both if the site should
ever become searchable.
