# craftpoker-site

The static marketing and blog site for **craftpoker.com**, built with
[Zola](https://www.getzola.org/) and deployed to
[Cloudflare Pages](https://pages.cloudflare.com/).

This site is **standalone and fully decoupled from the poker game**. It is
plain marketing content (homepage, mission, contact, and a blog with
per-stakeholder tag feeds). The live game runs separately at
**friends.craftpoker.com**. This repository is **NOT** a submodule of the
mb2 / rust-bucket game repo — do not vendor it there.

## Structure

```
config.toml                 # Zola config (base_url, feeds, taxonomies)
content/                    # Markdown content
  _index.md                 # marketing homepage
  mission.md                # Our Mission page
  contact.md                # Contact page
  blog/                     # blog section + posts
templates/                  # Tera templates
static/                     # static assets (images, etc.)
bin/deploy_site             # build + deploy helper
```

## Local preview

Install Zola (`brew install zola`), then:

```sh
zola serve      # live-reloading dev server at http://127.0.0.1:1111
zola build      # one-off build into ./public
zola check      # validate content and internal links
```

## Deploy

Two options:

1. **Script deploy:** run `bin/deploy_site`. It runs `zola build` and then
   `npx wrangler pages deploy public --project-name=craftpoker-site`. This
   requires Zola installed and a Cloudflare API token available to wrangler.

2. **Cloudflare Pages git-build (no local CI):** connect this repo to a
   Cloudflare Pages project and let Cloudflare build on push. Set the build
   command to `zola build`, the output directory to `public`, and **pin
   `ZOLA_VERSION`** in the Pages build settings (environment variables) so
   builds are reproducible.

DNS / apex (`craftpoker.com`) binding is handled separately (ops bead), not
here.

## Feeds

`generate_feeds = true` with `feed_filenames = ["atom.xml"]` produces a
site-wide feed at `/atom.xml`, a blog-section feed at `/blog/atom.xml`, and a
per-tag feed at `/tags/<tag>/atom.xml` for each stakeholder tag
(`players`, `investors`, `kickstarters`, `developers`).

---

_Original placeholder note (kept for provenance): This file started as a
placeholder so there was something for the first commit._
