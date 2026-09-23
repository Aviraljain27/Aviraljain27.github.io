# Aviral Jain — Portfolio

A static, no-build-step personal site (`index.html`, `style.css`, `script.js`). Deploys to GitHub Pages with zero configuration.

## Deploy to GitHub Pages

1. On github.com, create a new **public** repository named exactly `Aviraljain27.github.io` (this exact name puts the site at the root of your GitHub domain). Don't initialize it with a README/gitignore/license — this folder already has files.
2. From this folder, run:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/Aviraljain27/Aviraljain27.github.io.git
   git push -u origin main
   ```
   If `git commit` complains about missing identity, run `git config user.name "Aviral Jain"` and `git config user.email "aviraljain2712@gmail.com"` first (add `--global` if you want that identity for all repos, not just this one).
3. On GitHub: repo → **Settings → Pages** → under "Build and deployment", set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)` → Save.
4. Your site goes live in ~1 minute at **https://Aviraljain27.github.io/**.

## Before you publish — things to update

- [ ] `assets/Aviral_Jain_Resume.pdf` is currently your AI-focused resume (leads with GenAI/RAG/LLM + CV) — matches the site's own "Computer Vision & Applied GenAI" positioning and the broadest slice of roles you're targeting. Swap in the ML-focused version instead if you shift toward more classical-ML/stats roles.
- [ ] All four featured projects are now marked confidential/employer-owned. If you ever build and publish a personal open-source project, add a new project card for it with a real GitHub link — don't reuse a placeholder link on work you don't own the code to.
- [ ] Add a custom domain later via repo → Settings → Pages → Custom domain, if you buy one.

## Local preview

Any static file server works, e.g.:
```bash
python -m http.server 8000
```
then open `http://localhost:8000`.
