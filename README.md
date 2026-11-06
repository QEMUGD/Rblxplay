# Rblxplay

A Roblox game search and launcher with a 2016-inspired interface.

## Deploy with GitHub Pages
The workflow in `.github/workflows/pages.yml` deploys the repository root whenever you push to `main`.

After the first workflow succeeds, open **Settings → Pages** in the repository to confirm the deployment URL.

## Notes
- Search uses Roblox's public Omni Search endpoint.
- Game metadata (creation date, player count, visits) is requested from Roblox's public games API.
- Browser CORS/network restrictions may prevent direct API access; a backend proxy may be needed if that happens.
- The unavailable-games filter only detects unavailable states when Roblox exposes a status in returned public data. It cannot reveal removed experiences or bypass Roblox access restrictions.
