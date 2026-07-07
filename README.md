# Reckon — Bill Split App

Single-file web app that reads grocery/DoorDash receipts and splits bills.

## Structure

```
wrangler.jsonc      <- tells Cloudflare to serve the public/ folder as a static site
public/
  index.html        <- the entire app (React, spreadsheet engine, OCR all built in)
```

## How it deploys

Cloudflare runs `wrangler deploy`, reads `wrangler.jsonc`, sees the `assets.directory`
points to `./public`, and serves `public/index.html` as the homepage. No build step,
no framework, no npm install needed.

## To update the app

Replace `public/index.html` with a new version and commit. Cloudflare auto-redeploys.
