# Eye Atelier

Website for Eye Atelier — a high-end optical boutique at the Shoppes of Old Bridge, NJ.

## Deploy

This is a static site. Any static host will work — recommended flow:

1. Push this repo to GitHub
2. Connect to Vercel (vercel.com/new) — select the repo
3. Vercel auto-detects it as static and deploys to `*.vercel.app`
4. Add your custom domain under Project → Settings → Domains

## Editing

- **Small copy tweaks**: edit `index.html` directly in GitHub's web UI (pencil icon). Commit → Vercel redeploys in ~30 seconds.
- **New images**: drop into `assets/` or `assets/frames/`, reference from HTML.
- **Local preview**: any static server works. Quickest:
  ```
  npx serve .
  ```

## Structure

- `index.html` — the entire site (single file)
- `assets/` — brand + store photography
- `assets/frames/` — individual frame images for brand cells
- `vercel.json` — clean URLs + cache headers for assets

## Notes

- Mobile-first: 90% of traffic is expected from mobile
- All tap targets sized ≥44px; sticky Call/Book bar on mobile
- Address links open Google Maps directly
- Phone number uses `tel:` links for one-tap calling
