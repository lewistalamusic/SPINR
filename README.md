# Spinner

Turn any artwork into a spinning record video — ready for Instagram, TikTok, and YouTube.

## Deploy to GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to **Deploy from a branch** → `main` / `root`
4. Your site will be live at `https://yourusername.github.io/spinner/`

## Custom domain (optional)

To use a custom domain like `spinner.floodlitmedia.co.uk`:

1. Add a `CNAME` file containing just the domain name
2. In your DNS, add a CNAME record pointing to `yourusername.github.io`
3. In GitHub Pages settings, enter your custom domain

## Notes

- The entire app is a single `index.html` file — no build step, no dependencies
- Payments (Stripe / Apple Pay) are mocked in this prototype — a live version needs a small backend
- Video rendering happens client-side via `canvas.captureStream()` + `MediaRecorder`
- Pre-rendering starts in the background as soon as artwork + audio are uploaded
