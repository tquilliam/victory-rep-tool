# Victory Rep Product Tool

Internal product tool for Victory Curtains & Blinds consultants.

- Single static file (`index.html`). No build step, no server.
- All product data is read live from the Google Sheet on page load.
  To change content, edit the sheet — no redeploy needed.
- Falls back to built-in data if the sheet can't be reached (e.g. poor signal in a home).

## Hosting (GitHub Pages)
1. Push this folder to a repo.
2. Settings > Pages > Build and deployment > Deploy from a branch > `main` / `/ (root)`.
3. Site goes live at https://<user>.github.io/<repo>/

## Note on access
GitHub Pages sites are PUBLIC, even from a private repo (private Pages needs GitHub Enterprise).
This tool contains rep-only content (objection handling, pricing guidance, rep leaderboard).
If that matters, host on Cloudflare Pages + Cloudflare Access instead, which gives real login control.
