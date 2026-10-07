# StellantAI Astro templates

Free Astro and EmDash site starters. The Node.js templates in [`templates/`](templates) are the source catalog for the [EmDash Docker browser launcher](https://github.com/StellantAI/emdash-docker). Choose a template there, connect an empty GitHub site repository, and the launcher copies the selected template into that repository before building its Docker editor.

| Template | Node.js | Cloudflare |
| --- | --- | --- |
| Blank | [`templates/blank`](templates/blank) | — |
| Starter | [`templates/starter`](templates/starter) | [`templates/starter-cloudflare`](templates/starter-cloudflare) |
| Blog | [`templates/blog`](templates/blog) | [`templates/blog-cloudflare`](templates/blog-cloudflare) |
| Marketing | [`templates/marketing`](templates/marketing) | [`templates/marketing-cloudflare`](templates/marketing-cloudflare) |
| Portfolio | [`templates/portfolio`](templates/portfolio) | [`templates/portfolio-cloudflare`](templates/portfolio-cloudflare) |

The Node.js variants use local SQLite and file storage. The Cloudflare variants are included as upstream reference projects but are not offered in the Docker launcher. The launcher reads [`templates/catalog.json`](templates/catalog.json) and pins this repository's Git commit when it copies a template. The catalog pins the tested EmDash release (`1.2.0` in this snapshot) alongside the template source.

## Source and license

The template directories are copied from [`emdash-cms/templates`](https://github.com/emdash-cms/templates) commit [`1930243108073ebb41ff48533678af7635b01c37`](https://github.com/emdash-cms/templates/tree/1930243108073ebb41ff48533678af7635b01c37). The three homepage preview screenshots come from [`emdash-cms/emdash`](https://github.com/emdash-cms/emdash) commit [`0a929da1b4de80c7f82f23458c2b6282455062bb`](https://github.com/emdash-cms/emdash/tree/0a929da1b4de80c7f82f23458c2b6282455062bb/assets/templates). Upstream EmDash is MIT licensed; see [`templates/EMDASH-LICENSE.txt`](templates/EMDASH-LICENSE.txt). Review the provenance before adding third-party themes or images.

This repository is a snapshot, not an automatic upstream mirror. Changes to the templates, catalog, or previews should be reviewed together so the launcher shows the design it installs.
