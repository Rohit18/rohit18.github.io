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
- Research, datasets, full publications, contributions, and original background sections all remain on the homepage.
- Shared publication records: `_data/publications.json`; title, journal, and year links use `_includes/paper_reference.html`.
- Shared navigation: `_includes/site_header.html`, `_includes/site_footer.html`
- Base HTML shell: `_layouts/default.html`
- Navbar/footer link data: `_data/home.yml`
- Stylesheet: `assets/css/main.scss`
- Images: `images/`

## CV maintenance

The download at `assets/RohitMukherjeeCV.pdf` is built from `_cv/RohitMukherjeeCV.tex`.
The September 2026 version preserves the supplied CV and restores the Githu et al.
humanitarian-assistance paper from the existing website, with specific UFO and
vegetation-preprint links. The original files in the separate CV workspace are unchanged.

Compile the source with XeLaTeX into a temporary directory, inspect the rendered
pages, and copy the resulting PDF to `assets/RohitMukherjeeCV.pdf`.

Publication data and CV source should be updated together when manuscript statuses change.

## Notes

- Current and earlier projects, including Data, sit under Research. Existing images and older sections remain on the same scrolling page.
- Legacy Moonwalk theme files and plugin/theme dependencies have been removed.
