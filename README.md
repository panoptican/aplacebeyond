# A PLACE BEYOND

Minimal single-page ambient site with a looping video background and embedded audio player.

## Project Structure

- `index.html` - Main page with inline styles and media player markup.
- `generativeBG.mp4` - Fullscreen background video.
- `blackmoon.mp3` - Audio track played in the on-page player.
- `wrangler.toml` - Cloudflare Pages deployment configuration.

## Local Preview

Open `index.html` directly in your browser, or run a local static server.

Example with Python:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## Deploy to Cloudflare Pages

This repo is configured for static deployment with Wrangler.

```bash
npx wrangler pages deploy . --project-name aplacebeyond
```

## GitHub + Cloudflare Auto Deploy

Recommended production branch is `main`.
GitHub Actions workflow is configured at `.github/workflows/deploy-cloudflare-pages.yml` to deploy on push to `main`.

Set these repository secrets in GitHub:

- `CLOUDFLARE_API_TOKEN`
- `CLOUDFLARE_ACCOUNT_ID`
