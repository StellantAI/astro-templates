# StellantAI Astro templates

Free Astro and EmDash starters live under two template types: [`templates/website`](templates/website) for websites and [`templates/app`](templates/app) for apps. The Node.js website templates are the source catalog for the [LibreApps Dashboard](https://github.com/StellantAI/emdash-docker). Choose a website template there, connect an empty GitHub repository, and the Dashboard copies the selected template into that repository before building its Docker editor.

| Template | Node.js | Cloudflare |
| --- | --- | --- |
| Blank | [`templates/website/blank`](templates/website/blank) | — |
| Starter | [`templates/website/starter`](templates/website/starter) | [`templates/website/starter-cloudflare`](templates/website/starter-cloudflare) |
| Blog | [`templates/website/blog`](templates/website/blog) | [`templates/website/blog-cloudflare`](templates/website/blog-cloudflare) |
| Marketing | [`templates/website/marketing`](templates/website/marketing) | [`templates/website/marketing-cloudflare`](templates/website/marketing-cloudflare) |
| Portfolio | [`templates/website/portfolio`](templates/website/portfolio) | [`templates/website/portfolio-cloudflare`](templates/website/portfolio-cloudflare) |

The Node.js variants use local SQLite and file storage. The Cloudflare variants are included as upstream reference projects but are not offered in the Docker wizard. The Dashboard reads [`templates/catalog.json`](templates/catalog.json) and pins this repository's Git commit when it copies a website template. The catalog pins the tested EmDash release (`1.2.0` in this snapshot) alongside the template source. The app category currently contains a [`LibreApp/StellantAI` placeholder](templates/app/LibreApp/StellantAI); it is not runnable. No source from the private `StellantAI/client` repository is included.

## Source and license

Starter, Blog, Marketing, Portfolio, and their Cloudflare variants are copied from [`emdash-cms/templates`](https://github.com/emdash-cms/templates) commit [`1930243108073ebb41ff48533678af7635b01c37`](https://github.com/emdash-cms/templates/tree/1930243108073ebb41ff48533678af7635b01c37). The mirror’s Blank folder is a placeholder, so the runnable Blank template is copied from [`emdash-cms/emdash`](https://github.com/emdash-cms/emdash/tree/b5f37c646f3639f07ebdc090e0ffcf48bdb4d684/templates/blank) at the tested `1.2.0` release commit. The three homepage preview screenshots come from [`emdash-cms/emdash`](https://github.com/emdash-cms/emdash) commit [`0a929da1b4de80c7f82f23458c2b6282455062bb`](https://github.com/emdash-cms/emdash/tree/0a929da1b4de80c7f82f23458c2b6282455062bb/assets/templates). Upstream EmDash is MIT licensed; see [`templates/website/EMDASH-LICENSE.txt`](templates/website/EMDASH-LICENSE.txt). Review the provenance before adding third-party themes or images.

This repository is a snapshot, not an automatic upstream mirror. Changes to the templates, catalog, or previews should be reviewed together so the Dashboard shows the design it installs.
