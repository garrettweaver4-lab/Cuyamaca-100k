# Cuyamaca 100K Timing & Crew Plan

A single-page static web app for race-day timing, aid-station projections, crew coordination, fueling, gear, and live pace re-projection.

## Deploy to GitHub Pages

1. Create a GitHub repository and push the contents of this folder to the `main` branch.
2. In **Settings → Pages**, set the source to **GitHub Actions**.
3. The included workflow (`.github/workflows/deploy-pages.yml`) will deploy the site automatically on pushes to `main`.

GitHub Pages requires the site entry file (`index.html`) to be at the root of the published artifact.

## Deploy to Netlify

### Git deployment
Import this repository in Netlify. The included `netlify.toml` sets the publish directory to the repository root; no build command is required.

### Drag and drop
You can also drag this entire folder into Netlify's manual deploy area.

## Deploy to Vercel

Import the repository into Vercel. This is a static site, so no build command is required. The included `vercel.json` provides basic response headers.

## Local use

Open `index.html` directly in a modern browser. The app stores race-day logs in browser `localStorage`, so those logs remain on that browser/device until cleared.

## Notes

The site is intentionally kept as a static, dependency-light package. The original app's external Google Fonts stylesheet remains in `index.html`; the application JavaScript and CSS are embedded in the page itself.
