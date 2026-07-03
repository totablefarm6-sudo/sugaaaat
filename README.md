# Saugaat Farms — Website

A single-page site for Saugaat Farms (fresh farm products from Sindh & Multan). Pure HTML/CSS/JS — no build step, no dependencies.

## Project structure

```
saugaat-farms/
├── index.html      # the whole site
├── vercel.json      # static site config for Vercel
├── .gitignore
└── README.md
```

## Put it on GitHub

1. Create a new repo on GitHub (e.g. `saugaat-farms`) — don't add a README/license there, we already have one.
2. In this folder, run:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Saugaat Farms website"
   git branch -M main
   git remote add origin https://github.com/<your-username>/saugaat-farms.git
   git push -u origin main
   ```

## Deploy on Vercel (no config needed)

**Option A — via GitHub (recommended, auto-deploys on every push):**
1. Push the repo to GitHub (steps above).
2. Go to https://vercel.com/new
3. Import the `saugaat-farms` repo.
4. Framework preset: **Other** (it's static HTML, Vercel detects this automatically).
5. Leave build command / output directory blank — click **Deploy**.
6. Your site goes live at `https://saugaat-farms-<something>.vercel.app` (you can add a custom domain in Project Settings → Domains).

**Option B — instant deploy from your computer, no GitHub needed:**
```bash
npm i -g vercel
cd saugaat-farms
vercel --prod
```
Follow the prompts (log in, confirm project name) and it deploys straight to a live URL.

## Notes
- All images currently load from Unsplash URLs — fine for launch, but for production you may want to download and self-host them in an `/images` folder for reliability and speed.
- WhatsApp, Instagram, and Facebook links are already wired up in the Contact and top ribbon sections.
