# genbasic.com

The GenBasic brand site. Static, built by **GitHub Pages' native Jekyll** — no
Actions workflow, no plugins outside the Pages default set, and no remote theme,
so a push to `master` is the whole deploy.

## Layout

| Path | What it is |
|---|---|
| `_config.yml` | Site metadata. Plugins deliberately empty. |
| `index.md` | The landing page. |
| `_layouts/default.html` | The only layout; self-contained. |
| `assets/css/main.css` | All styling. Light + dark via `prefers-color-scheme`. |
| `CNAME` | `genbasic.com` — routes the custom domain to this repo. |

## Local preview

```sh
gem install bundler jekyll
jekyll serve      # http://127.0.0.1:4000
```

## DNS

`genbasic.com` is on Cloudflare. The apex carries GitHub Pages' four `A` and
four `AAAA` records and `www` is a `CNAME` to `genbasic.github.io` — all
**DNS-only** (grey cloud), which is what lets GitHub issue the TLS certificate.

The `wiki`, `forum` and `shop` subdomains are separate services and are not
touched by this repo.
