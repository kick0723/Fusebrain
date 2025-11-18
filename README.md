# Fusebrain

This repository contains a small static site package for "FuseBrain AI". It is a static site (no build step required). The important file is `index.html`.

**Quick Preview (local)**

1. Serve with Python from the repository root:

```bash
# from repo root
python3 -m http.server 8000
# open http://localhost:8000/
```

2. Or use `live-server` (if installed):

```bash
npm i -g live-server
live-server --port=3000
```

**Make site root-friendly**

If the main file is named `website.html`, rename it to `index.html` so the root URL serves the site:

```bash
mv website.html index.html
```

**Docker (optional)**

A simple `Dockerfile` is included to serve the site with Nginx. To build and run:

```bash
docker build -t fusebrain-site .
docker run --rm -p 8080:80 fusebrain-site
# open http://localhost:8080/
```

**Publish**

- GitHub Pages: rename to `index.html`, commit, and enable Pages from the repository `main` branch (root).
- Netlify / Vercel: connect the repo or drag-and-drop the build folder to deploy a static site.

**Repository files**

- `index.html` - site HTML
- `branding.txt`, `business_plan.txt`, `terms_of_service.txt`, `privacy_policy.txt`, `refund_policy.txt`, `training_prompt.txt`, `marketing_assets.txt`, `onboarding.txt`, `email_sequences.txt`, `pricing.txt` - doc assets
- `Dockerfile` - simple Nginx server for containerized serving

If you want, I can:

- start a local Python server and leave it running
- build and run the Docker image here and show the result (if Docker daemon is available)
- commit these changes and open a PR

Tell me which of those you'd like next.
# Fusebrain