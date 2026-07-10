# opte.ch

Static site for [opte.ch](https://opte.ch), built with [Hugo](https://gohugo.io) and the
[Congo](https://jpanther.github.io/congo/) theme, hosted on GitHub Pages.
Migrated from Squarespace in July 2026 — all legacy URLs (posts, tags, categories)
redirect to their new locations via Hugo aliases.

## One-time setup

```sh
brew install hugo
git clone --recurse-submodules git@github.com:mikeoertli/mikeoertli.github.io.git
```

If you already cloned without submodules (the theme lives in `themes/congo`):

```sh
git submodule update --init --recursive
```

## Local preview

From the repo root:

```sh
hugo server
```

Then open <http://localhost:1313>. The server watches for changes and live-reloads;
press `Ctrl+C` to stop it.

To preview from another device on the tailnet (e.g. an iPad while this runs on
`maxbookpro`):

```sh
hugo server --bind 0.0.0.0 --baseURL http://maxbookpro:1313/ --appendPort=false
```

Then open <http://maxbookpro:1313> on the other device.

## Editing content

| What | Where |
|---|---|
| Homepage / consulting pitch | `content/_index.md` |
| Recommendations | `content/tech-picks/index.md` |
| Contact page (Formspree form) | `content/contact.md` |
| Blog archive posts | `content/news/<slug>/index.md` |
| Author name/photo/links, site title | `config/_default/languages.en.toml` |
| Theme behavior (search, dark mode, lists) | `config/_default/params.toml` |
| Header/footer menus | `config/_default/menus.en.toml` |

Posts are page bundles: each post's images live in its own directory next to its
`index.md`. A `feature.*` image in a bundle becomes the post's cover / link-preview
image (thumbnails are intentionally hidden on list pages via the override in
`layouts/_partials/article-link.html`).

The `content/tags/` and `content/categories/` directories hold generated term pages
whose only job is redirecting legacy Squarespace URLs — leave them alone unless
removing a tag entirely.

## Deploying

Every push to `main` triggers `.github/workflows/hugo.yml`, which builds the site
and deploys it to GitHub Pages. There is nothing to build or commit locally —
never commit the `public/` directory (it's gitignored).

To update the Congo theme:

```sh
git submodule update --remote themes/congo
git add themes/congo && git commit -m "Update Congo theme"
```

## Migration artifacts

The Squarespace crawl data and conversion scripts live outside this repo in
`~/develop/optech/migration_claude/` (crawl JSON, `convert.py`,
`gen_taxonomy_aliases.py`). They are only needed if content ever has to be
re-extracted; re-running `convert.py` will overwrite hand-edits to migrated
content files.
