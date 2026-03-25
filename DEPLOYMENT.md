# cheori-ad-preview deployment notes

This repository is structured for GitHub Pages with a single root file:

- `index.html` in the repository root.

## What is already ready

- The site entry point is `index.html` at root (required for Pages from branch + root).
- The ad creatives are embedded as data URIs, so there are no required local asset files.
- External CDN references remain intact inside embedded ad payloads.

## Publish steps (manual)

Run these commands from this repo after creating your GitHub repo:

```bash
git branch -M main
git remote add origin https://github.com/<YOUR_USERNAME>/cheori-ad-preview.git
git push -u origin main
```

Then in GitHub:

1. Open `Settings` → `Pages`.
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
3. Set **Branch** to `main` and **Folder** to `/ (root)`.
4. Click **Save**.

Your site will publish at:

`https://<YOUR_USERNAME>.github.io/cheori-ad-preview/`

(Initial deployment can take a few minutes.)
