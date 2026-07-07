# Reckon — Bill Split App

Single-file web app that reads grocery/DoorDash receipts and splits bills.

## Structure

```
wrangler.jsonc      <- tells Cloudflare to serve the public/ folder as a static site
public/
  index.html        <- the entire app (React, spreadsheet engine, OCR all built in)
```
