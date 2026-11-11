# Personal website (Quarto)

Source for https://www.thomaspuschel.com, rebuilt with [Quarto](https://quarto.org) from the earlier blogdown/Hugo Academic site. It shares its theme with the lab site (https://cea-lab.org).

## Preview locally

```bash
quarto preview
```

## Add a publication

1. Copy an existing folder in `publication/` (for example `publication/pnas_2026/`) and rename it. The folder name becomes the URL.
2. Edit `index.qmd`: `title`, `subtitle` (authors), `date`, `description` (journal line), `categories` (type first, then tags), `doi`.
3. Optional: add `featured.jpg` and set `image: featured.jpg`; put the PDF in `files/pdf/`; set `featured: true` to show it under Featured Publications on the home page.

Talks (`talk/`), research projects (`project/`) and posts (`post/`) work the same way.

## Notes

- The R tutorials in `post/` embed the HTML that blogdown rendered, so the site builds without R. The `.Rmd` sources sit next to each post for download.
- `.github/workflows/deploy.yml` renders and publishes to GitHub Pages on every push to `main`.
