# barnisan.com

Official website for **Barnisan LLC** — hosted on GitHub Pages.

## Files

- `index.html` — the site (single file, no build step, no dependencies)
- `404.html` — not-found page
- `CNAME` — tells GitHub Pages this repo serves `barnisan.com`

## Deploy (GitHub Pages)

1. Create a new **public** repo on this account (e.g. `barnisan.com`).
2. Upload `index.html`, `404.html`, and `CNAME` to the repo root (main branch).
3. Repo **Settings → Pages** → Source: *Deploy from a branch* → Branch: `main`, folder `/ (root)` → Save.
4. Under **Custom domain**, enter `barnisan.com` → Save.
5. Once DNS (below) has propagated, check **Enforce HTTPS**.

## DNS (at the registrar where barnisan.com lives)

Apex `barnisan.com` — four **A** records:

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

`www` — one **CNAME** record pointing to:

```
aly-wh.github.io
```

Propagation is usually minutes, occasionally up to 24h. The "Enforce HTTPS"
checkbox becomes available once GitHub has issued the certificate.
