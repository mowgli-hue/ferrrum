# Ferrum Sheet Metal — Website

Static one-page site. Two files: `index.html` (the site) and `vercel.json` (config).

---

## Deploy to Vercel — Easiest Way (drag & drop, no coding)

1. Unzip `ferrum-website.zip` on your computer. You'll get a folder with `index.html` and `vercel.json` inside it.
2. Go to **https://vercel.com/signup** and sign up (free — use Google or GitHub login).
3. Once you're in your dashboard, click **"Add New..."** → **"Project"**.
4. Look for an option that says **"deploy a template"** or scroll down — you want **"Deploy without a Git repository"** OR install the Vercel CLI (see below).

> Tip: If the dashboard doesn't show drag-and-drop, the easiest path is the CLI method below — it takes 60 seconds.

---

## Deploy with Vercel CLI (recommended — fastest)

Open Terminal (Mac) or PowerShell (Windows) and run:

```bash
# 1. Install Vercel CLI (one-time)
npm install -g vercel

# 2. Go into the unzipped folder
cd path/to/ferrum-website

# 3. Deploy
vercel
```

It will ask you a few questions — press Enter to accept defaults for all of them. After ~30 seconds you'll get a live URL like `ferrum-website-xxx.vercel.app`.

To make it the production deployment, run:

```bash
vercel --prod
```

> Don't have Node/npm? Install it from https://nodejs.org (pick the LTS version), then come back to step 1.

---

## Adding Your Custom Domain

Once the site is deployed:

1. In your Vercel dashboard, click your project → **Settings** → **Domains**.
2. Click **"Buy"** to purchase a domain through Vercel (e.g. `ferrumsheetmetal.com`, `ferrum.ca`, etc.) OR type a domain you already own and follow the DNS instructions.
3. Vercel will auto-configure SSL (https) — usually live in a couple minutes.

Domain suggestions for this business:
- `ferrumsheetmetal.com`
- `ferrumsheetmetal.ca` (Canadian — recommended)
- `ferrummetal.ca`
- `ferrumbc.ca`

---

## Updating the Site Later

Just edit `index.html`, then run `vercel --prod` again from the folder. Done.

If you want a no-terminal workflow, push the folder to a GitHub repo and connect it to Vercel — every change you save will auto-deploy.

---

## What's Inside

- **`index.html`** — the entire website (HTML + CSS + a tiny bit of JS, all inlined)
- **`vercel.json`** — tells Vercel to serve clean URLs and adds basic security headers
