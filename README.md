# muse

The Muse puff piece — a local briefing site for the personal AI agent
line from Meta, in the filed.fyi "puff pieces" series. Sibling to
[grok.filed.fyi](https://grok.filed.fyi/).

Built with [boris](https://github.com/drawmeanelephant/boris), a Zig
static-site compiler. Deploys to <https://muse.filed.fyi/> via
Cloudflare Pages on push to `main`.

```sh
# zero-write preflight
boris validate --input content --theme lab \
  --layout-rule default id:index lab/layouts/trunk.html --static-dir static

# full build
boris build --input content --html-dir dist \
  --theme lab --sitemap --site-url https://muse.filed.fyi/ \
  --layout-rule default id:index lab/layouts/trunk.html --static-dir static
```

## Brand mark review

The hand-authored masters and browser previews are:

- Fart Knocker: [`SVG`](static/brand/fart-knocker.svg) /
  [`preview`](static/brand/index.html).
- Oliver: [`SVG`](static/brand/oliver.svg) /
  [`preview`](static/brand/oliver.html), based on the supplied Oliver favicon reference.

Each preview shows 16 / 32 / 64 / 256 px on light and dark backgrounds
and a large render. Oliver's preview also shows the two marks side by side.
Open the HTML files directly, or after a full build open `dist/brand/index.html`
and `dist/brand/oliver.html`. The deployed paths are `/brand/` and `/brand/oliver.html`.

No SVG editor or extra packages are required: edit the SVG as text and
refresh the preview. Both marks have the owner's visual approval for
issues #1 and #2. The current avatar and favicon are unchanged;
shipping the Oliver mark to its own repo remains a separate handoff.
