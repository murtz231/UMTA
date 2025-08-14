# UMTA Static Site (Vercel-ready)

This repository hosts the Undergraduate Mock Trial Association website as a single static page.

## Deploy on Vercel (Git flow)

1. Create a new repository:
   ```bash
   git init
   git add .
   git commit -m "initial commit: static site"
   ```
2. Create a repo on GitHub/GitLab/Bitbucket and add it as the remote:
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/umta-site.git
   git push -u origin main
   ```
3. Go to https://vercel.com > **Add New Project** > **Import Git Repository** > pick your repo.
4. Framework preset: **Other** (no framework). Build command: **None**. Output directory: **/** (root).
5. Click **Deploy**.

## Deploy on Vercel (CLI)

```bash
npm i -g vercel
vercel  # follow the prompts; when asked for framework, choose “Other” and output dir “/”
```

## Project structure

```
.
├─ index.html       # your site (inline CSS/JS; no build step required)
└─ vercel.json      # minimal config (optional)
```

> Contact form uses `mailto:`; it opens the visitor's email client instead of sending from the site.
