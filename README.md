# nordingpartners.no

The Nording & Partners website: a single static page, no build step, no dependencies.

## Structure

```
index.html              the page
favicon.svg             N&P monogram
assets/css/site.css     all styles (design tokens at the top)
assets/img/             hero photo, logos, team portraits (assets/img/team/)
assets/fonts/           Noto Sans (body) and Gelasio (Georgia fallback), self-hosted, OFL licence
robots.txt, sitemap.xml
```

## Editing

- **Text**: edit `index.html` directly. Every section is marked with a comment-free, readable structure (`.hero`, `.intro`, `.work`, `.team`, `.careers`, `.contact`).
- **Team**: each person is one `<article class="person">` block. Replace the portrait at `assets/img/team/<initials>.jpg` (1280 × 800, 8:5, black and white, person on the right third) and update name, role, bio and contact.
- **Colours and spacing**: the `:root` block at the top of `assets/css/site.css`.

## Preview locally

Any static server works, e.g.

```
python3 -m http.server 8000
```

then open http://localhost:8000.

## Hosting

Static hosting with a custom domain: GitHub Pages, Cloudflare Pages or Netlify. Point `www.nordingpartners.no` (CNAME) and the apex at the host; email records are unaffected.

## Design source

The page was designed on a Claude Design canvas against the "Nording & Partners — Rebrand" design system (navy #101b2a, steel #4579a0, stone #c0c3bb; Georgia headings, Noto Sans text; hairlines, no boxes).
