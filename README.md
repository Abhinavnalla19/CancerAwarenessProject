# Cancer Awareness & Support

A simple static site to promote cancer awareness, hope, and support.

## Project structure
- `index.html` — Single-page site with a hero header, banner image, inspirational quote (fetched from Quotable API), and a contact form.

## Run locally

- Easiest: double-click `index.html` to open in your browser.
- Recommended (local server):

```powershell
cd e:\CancerAwarenessProject; python -m http.server 8000
# then visit http://localhost:8000
```

## Deploy options

### GitHub Pages (static hosting)
1. Push this repo to GitHub (already done).
2. In the repo Settings → Pages:
   - Source: Deploy from a branch
   - Branch: `main` and folder `/root`
3. Save. Your site will be published at `https://<username>.github.io/<repo>/`.

### Netlify (optional)
1. Go to https://app.netlify.com/ → Add new site → Import from Git.
2. Choose this repo. For a static HTML site:
   - Build command: (leave empty)
   - Publish directory: `.`
3. Deploy.

## Notes
- Quotes are fetched from `https://api.quotable.io/random`. If offline, the page shows a fallback message.
- The contact form currently uses a simple alert and reset; connecting it to a backend or Netlify Forms requires minor changes.
