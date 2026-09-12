# nifraworld.com — landing site

Static site. No build step.

```
index.html      landing page (SEO meta, Open Graph, JSON-LD included)
privacy.html    DRAFT privacy policy — review before publishing
robots.txt
sitemap.xml
assets/         app icons, favicon; add og-nifraworld.png (1200×630), logo-512.png, apple-touch-icon.png (180×180)
```

## Deploy (Cloudflare Pages, same place the apps live)

1. Cloudflare dashboard → Workers & Pages → Create → Pages → **Upload assets** (or connect a Git repo) → upload this `site/` folder.
2. Project → Custom domains → add `nifraworld.com` **and** `www.nifraworld.com`. Cloudflare creates the DNS records.
3. Rules → Redirect Rules → redirect `www.nifraworld.com/*` → `https://nifraworld.com/$1` (301).
4. Verify: `https://nifraworld.com` loads, `https://nifraworld.com/robots.txt` and `/sitemap.xml` load.

## Before going live — three placeholders to fill

- `https://www.facebook.com/nifraworld` — claim this username on the Facebook page (Page settings → Username), or replace every occurrence with the page's real URL.
- `assets/og-nifraworld.png` — 1200×630 share image. Without it Facebook shows a blank card.
- `privacy.html` — remove the yellow draft box once reviewed.

## After going live

- Google Search Console → add property `nifraworld.com` (Domain type, DNS TXT record in Cloudflare) → submit `sitemap.xml`.
- Bing Webmaster Tools → import from Search Console.
- Facebook Sharing Debugger (developers.facebook.com/tools/debug) → paste `https://nifraworld.com/` → Scrape again.
