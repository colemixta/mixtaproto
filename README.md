# Mixta — "How It Works" Interactive Concept

A clickable prototype of a reworked **How It Works** section: a 4-step tab bar
(Build Your Scenario → Generate in Minutes → Distribute Instantly → Measure &
Improve) that replaces the current embedded generative-video demo. Clicking
any step enlarges it and reveals a GIF-preview panel below, showing what a
real product GIF for that step should contain.

This is a design concept only — the "GIF preview" panels are static mockups
labeled as content slots, not real product footage.

## View it locally

Just open `index.html` in any browser — no build step, no dependencies.

## Deploy to GitHub Pages

This repo is already structured for Pages with no build step required.

1. Push this repo to GitHub (see commands below).
2. In the repo on GitHub: **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Branch: **main**, folder: **/ (root)**. Click **Save**.
5. GitHub will publish the site at:
   `https://<your-username>.github.io/<repo-name>/`
   (takes 1–2 minutes on first deploy)

### Push commands

```bash
cd mixta-prototype
git init
git add .
git commit -m "Add How It Works interactive prototype"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

Then follow steps 2–5 above in the GitHub UI.

## Files

- `index.html` — the prototype (single file, inline CSS/JS, no external assets)
- `.nojekyll` — tells GitHub Pages to skip Jekyll processing (not needed for
  this file, but prevents edge-case issues if the repo grows)
- `.gitignore` — ignores OS junk files
