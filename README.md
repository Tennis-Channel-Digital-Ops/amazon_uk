# Amazon UK Live Monitor

TC UK live schedule browser for Amazon UK metadata.

## What it does

Single-page web UI (`index.html`) that shows the TC UK live feed schedule in three tabs:

- **Now Playing** — what's live right now
- **Upcoming** — scheduled future events
- **Finished** — historical airings with a date picker

It fetches data from `https://epg.incbrief.com/api` and supports timezone selection.

## Runtime

- Static HTML + Tailwind CSS + vanilla JavaScript
- No build step; serve the folder with any HTTP server
- Local dev: open `index.html` directly, or run `python3 -m http.server 8105`

## DOPS publication

| Item | Value |
|------|-------|
| Slug | `/amazon-uk/` |
| Port | `8105` |
| DOPS URL | `https://dops.tct2pbtv.com/amazon-uk/` |

Publish via DOPS Publisher Admin (`/publisher-admin`) and assign users in Auth Admin (`/auth-admin`).

## Source

GitHub: `https://github.com/Tennis-Channel-Digital-Ops/amazon_uk.git`

## Files

- `index.html` — the entire app
