# nifraworld.com — landing site

Static site, no build step. Deployed from GitHub via Cloudflare Pages (same flow as the apps).

```
index.html      landing page (SEO meta, Open Graph, JSON-LD for all three apps)
privacy.html    DRAFT privacy policy — owner must review, then remove the yellow box
robots.txt / sitemap.xml
assets/         og-*.png share images (1200x630), logo-512.png, apple-touch-icon.png, favicon.svg, app icons
```

## Status (12 Sep 2026)
- [x] Site built and committed locally (git, branch main)
- [x] Spelling Buddy repo: SEO head + og image pushed → live
- [x] Boithok Ghor repo: SEO head + og image + manifest pushed (verify live)
- [x] Khela Ghor: SEO head added to KHELA-GHOR-v2.5.4-DEPLOY (owner re-uploads folder)
- [ ] GitHub repo `nifraworld/nifraworld-site` created and pushed
- [ ] Cloudflare Pages project connected; custom domains nifraworld.com + www
- [ ] khelaghor.nifraworld.com custom domain on the khela-ghor project
- [ ] Facebook page: rename, @nifraworld, website, CTA, cover
- [ ] Search Console + Bing + Cloudflare Web Analytics
- [ ] Privacy draft reviewed; facebook.com/nifraworld confirmed or replaced

## Cloudflare Pages settings for this repo
Framework preset: None · Build command: (empty) · Build output directory: `/`
