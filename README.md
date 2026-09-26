# muse

The Muse puff piece — a local briefing site for the personal AI agent
line from Meta, in the filed.fyi "puff pieces" series. Sibling to
[grok.filed.fyi](https://grok.filed.fyi/).

Built with [boris](https://github.com/drawmeanelephant/boris), a Zig
static-site compiler. Deploys to <https://boris-muse.pages.dev/> via
Cloudflare Pages on push to `main`.

```sh
# zero-write preflight
boris validate --input content --theme lab \
  --layout-rule default id:index lab/layouts/trunk.html --static-dir static

# full build
boris build --input content --html-dir dist \
  --theme lab --sitemap --site-url https://boris-muse.pages.dev/ \
  --layout-rule default id:index lab/layouts/trunk.html --static-dir static
```
