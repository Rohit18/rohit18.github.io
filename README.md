# Rohit Mukherjee Website

Standalone Jekyll site for [rohitmukherjee.space](https://www.rohitmukherjee.space), with local layouts and styling (no external theme dependency).

## Stack

- Jekyll `~> 4.2`
- Local layouts in `_layouts/`
- Shared include: `_includes/horizontal_list.html`
- Site config in `_config.yml`

## Local Development

From the repository root:

```bash
bundle install
bundle exec jekyll serve --livereload
```

Open `http://127.0.0.1:4000`.

To build only:

```bash
bundle exec jekyll build
```

Output is generated in `_site/`.

## Content and Structure

- Homepage entrypoint: `index.md`
- Main homepage content: `_layouts/home.html`
- Base HTML shell: `_layouts/default.html`
- Navbar/footer link data: `_data/home.yml`
- Stylesheet: `assets/css/main.scss`
- Images: `images/`

## Notes

- This repo intentionally keeps only the files used by the current homepage-driven site.
- Legacy Moonwalk theme files and plugin/theme dependencies have been removed.
