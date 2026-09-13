# nifraworld.com — landing site

Static site, no build step. Deployed from GitHub via Cloudflare Pages (same flow as the apps).

```
index.html      landing page (SEO meta, Open Graph, JSON-LD for all three apps)
privacy.html    DRAFT privacy policy — owner must review, then remove the yellow box
robots.txt / sitemap.xml
assets/         og-*.png share images (1200x630), logo-512.png, apple-touch-icon.png, favicon.svg, app icons
```

## Status (13 Sep 2026) — Phase 0 complete
- [x] Site built and committed locally (git, branch main)
- [x] Spelling Buddy repo: SEO head + og image pushed → live
- [x] Boithok Ghor repo: SEO head + og image + manifest pushed (verify live)
- [x] Khela Ghor: SEO head added to KHELA-GHOR-v2.5.4-DEPLOY (owner re-uploads folder)
- [x] GitHub repo `nifraworld/nifraworld.com` created and pushed
- [x] Cloudflare Pages project connected; custom domains nifraworld.com + www (www 301 → apex)
- [x] Khela Ghor moved to GitHub (nifraworld/khela-ghor) + khelaghor.nifraworld.com
- [x] Facebook page: Nifra World, facebook.com/nifraworld, cover, bio, CTA
- [x] Search Console (all 4 URLs indexed 13 Sep) + Bing (4 URLs submitted) + Cloudflare Web Analytics on all hosts
- [x] Privacy reviewed and final at /privacy; facebook.com/nifraworld confirmed

## Cloudflare Pages settings for this repo
Framework preset: None · Build command: (empty) · Build output directory: `/`
