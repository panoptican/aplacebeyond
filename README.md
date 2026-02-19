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
When the Cloudflare Pages project is connected to GitHub, pushes to `main` trigger production deployments.
