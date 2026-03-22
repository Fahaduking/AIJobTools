# AIJobTools — Deployment Guide

## Project Structure
```
aijobtools/
├── index.html              ← Homepage
├── sitemap.xml             ← SEO sitemap
├── robots.txt              ← Search crawler rules
└── pages/
    ├── ai-tools-for-freelancers.html
    ├── ai-tools-for-students.html     (build next)
    ├── ai-tools-for-teachers.html     (build next)
    ├── ai-tools-for-marketers.html    (build next)
    ├── ai-tools-for-developers.html   (build next)
    ├── ai-tools-for-content-creators.html
    ├── free-ai-tools.html
    ├── chatgpt-vs-claude.html
    ├── blog.html
    └── about.html
```

## Deploy to GitHub Pages (FREE — no credit card)

### Step 1 — Create GitHub Account
1. Go to https://github.com
2. Sign up for free (no credit card)

### Step 2 — Create Repository
1. Click "New repository"
2. Name it exactly: `aijobtools` (or your-username.github.io for root domain)
3. Set to Public
4. Click "Create repository"

### Step 3 — Upload Files
Option A (Drag & Drop — easiest):
1. Click "uploading an existing file" in your new repo
2. Drag ALL files from this folder into the browser
3. Click "Commit changes"

Option B (Git command line):
```bash
git init
git add .
git commit -m "Initial site launch"
git remote add origin https://github.com/YOUR_USERNAME/aijobtools.git
git push -u origin main
```

### Step 4 — Enable GitHub Pages
1. Go to your repository → Settings
2. Click "Pages" in the left sidebar
3. Under "Source" → select "main" branch → "/" (root)
4. Click Save
5. Your site will be live at: https://YOUR_USERNAME.github.io/aijobtools/

### Step 5 — (Optional) Connect Cloudflare for speed
1. Sign up at https://cloudflare.com (free, no credit card)
2. Add your github.io URL as a custom domain
3. Cloudflare gives you: CDN, caching, HTTPS, faster loading

## After Launch — SEO Steps

1. Go to https://search.google.com/search-console
2. Sign in with Google
3. Add your site URL
4. Submit your sitemap: YOUR_URL/sitemap.xml
5. Google will start indexing your pages within 1-2 weeks

## Update the site URL
When live, replace all instances of:
  https://aijobtools.github.io/
with your actual URL in:
  - index.html (canonical tag)
  - all pages/ files (canonical tags)
  - sitemap.xml
