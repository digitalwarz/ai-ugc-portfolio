# Portfolio — Deploy Guide

> The portfolio is a self-contained static site in this folder: `index.html` + 4 videos. It turns "attach 4 files" into "here's one link" — the single URL to drop into every Upwork proposal and cold email.

## What's here
| File | Purpose |
|---|---|
| `index.html` | Single-page portfolio (dark + volt-green, matches Aurelius brand) |
| `demo-reel-sendable.mp4` | 30s reel, 720×1280, 8.3 MB |
| `ugc-skincare-serum-demo-ad.mp4` | 5s skincare sample |
| `ugc-supplement-demo-ad.mp4` | 5s supplement sample |
| `ugc-mens-grooming-demo-ad.mp4` | 5s men's grooming sample |

## Deploy options (pick one, ~2 min each)

### Option A — Netlify Drop (fastest, no account needed for a test)
1. Go to https://app.netlify.com/drop
2. Drag this entire `portfolio/` folder onto the page.
3. Get a `*.netlify.app` URL instantly. (Free account to keep it permanent + custom domain.)

### Option B — GitHub Pages (free, permanent, custom domain)
1. Create a repo, push this folder's contents to the root (or `/docs`).
2. Settings → Pages → deploy from branch.
3. URL: `https://<user>.github.io/<repo>/`.

### Option C — Vercel
1. `npx vercel` in this folder, or drag-drop at vercel.com/new.
2. Instant `*.vercel.app` URL.

## How to use the link
- **Upwork proposals:** paste the URL in the proposal body ("Portfolio: <url>") — clients click one link instead of downloading 4 attachments.
- **Cold email/WhatsApp:** one line — "Here's my reel: <url>".
- **The CTA on the page** already routes to `taahir@foreverlawn.co.za` with a "Request free plan" subject line, so inbound leads self-qualify.

## Note
The page's mailto CTA uses `taahir@foreverlawn.co.za`. If you'd rather route inbound to a different address (or a Wise/Upwork-linked inbox), change the two `mailto:` links in `index.html` before deploying.
