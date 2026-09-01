# Connor Randall — Portfolio Site

A static portfolio site (no build step, no dependencies) that hosts engineering
case studies and links to their PDF versions. Ready to deploy on GitHub Pages.

## Files

```
portfolio/
├── index.html                     Landing page (hero, selected work, contact)
├── styles.css                     Shared styles for all pages
├── work/
│   └── customer-health.html       Customer Health case study (web version)
├── assets/
│   └── CustomerHealth_CaseStudy.pdf   Downloadable PDF version
└── README.md                      This file
```

## One thing to edit before publishing

In `index.html`, find `YOUR-GITHUB-USERNAME` in the footer and replace it with
your actual GitHub username so the GitHub link works.

## Deploy on GitHub Pages (about 3 minutes)

You can either create a brand-new repo or drop these files into an existing one.

**Option A — a dedicated site at `https://<username>.github.io`:**
1. Create a repo named exactly `<username>.github.io`.
2. Put the *contents* of this `portfolio/` folder at the repo root
   (so `index.html` sits at the top level, not inside a `portfolio/` subfolder).
3. Commit and push to the `main` branch.
4. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   pick `main` and `/ (root)`, then Save.
5. Wait ~1 minute. Your site is live at `https://<username>.github.io`.

**Option B — a project page on an existing repo:**
1. Copy this `portfolio/` folder into the repo (or push it as its own repo, e.g. `portfolio`).
2. Enable Pages the same way (Settings → Pages → main branch).
3. The site will be at `https://<username>.github.io/<repo-name>/`.

## Put the link on your resume

Once live, add the URL to your resume header next to LinkedIn, e.g.:

`Mount Laurel, NJ · 856-669-1611 · cmrandall.business@gmail.com · linkedin.com/in/connormrandall · <your-portfolio-url>`

Keep it short — a `github.io` URL is fine, or add a custom domain later in
Settings → Pages if you want something like `connorrandall.dev`.

## What's included

Four complete case studies, each as a readable web page (`work/`) plus a
downloadable PDF (`assets/`):
- Customer Health — real-time integration monitoring
- Transaction API consolidation
- MariaDB → MySQL migration
- Audit-history pattern

## Adding a new case study later

1. Copy any file in `work/` (e.g. `work/customer-health.html`) to a new file and
   swap in its content and diagram; drop its PDF in `assets/`.
2. In `index.html`, duplicate one of the `<div class="entry">` blocks under
   "Selected work" and point its two links at the new page and PDF.
