# dashcsv-website

Standalone **DashCSV** product site — landing page, privacy policy, terms, support, and user guide.
Branded to match [dashwellsolutions.com](https://dashwellsolutions.com).

Published via **GitHub Pages** from the `docs/` folder on the **`main`** branch:

| Page | URL |
|------|-----|
| Home | https://nzj7bzjxr8-create.github.io/dashcsv-website/ |
| Privacy Policy | https://nzj7bzjxr8-create.github.io/dashcsv-website/privacy.html |
| Support | https://nzj7bzjxr8-create.github.io/dashcsv-website/support.html |
| Terms of Use | https://nzj7bzjxr8-create.github.io/dashcsv-website/terms.html |
| User Guide | https://nzj7bzjxr8-create.github.io/dashcsv-website/guide.html |

> ⚠️ **App Store Connect note:** `privacy.html` and `support.html` may be referenced as the app's
> Privacy/Support URLs. **Do not rename or delete them** — keep both live and returning HTTP 200.

## Edit and publish (no build step)

```bash
# 1. Edit any page or the stylesheet
#    docs/index.html  docs/privacy.html  docs/terms.html  docs/support.html  docs/guide.html  docs/style.css

# 2. Commit and push to the main branch
git add -A
git commit -m "Update DashCSV site"
git push                 # branch: main

# 3. GitHub Pages rebuilds docs/ automatically — live in ~1 minute.
```

There is **no build/CI step** — the HTML in `docs/` is served as-is.

## Look & feel

- Stylesheet `docs/style.css` matches dashwellsolutions.com (black hero, white `#e5e7eb`-bordered
  cards, 16px radius, Dashwell logo header, LLC footer). The canonical copy lives in the Dashwell
  repo at `web-shared/github-pages-style.css` — edit there, then copy into `docs/style.css` to keep
  both app sites consistent.
- Each page sets `<link rel="canonical">` to the matching `dashwellsolutions.com/dashcsv…` URL so the
  WordPress site stays the SEO-canonical source.
- Legal text mirrors `Dashwell/wordpress/dashcsv-*-content.txt`. When legal copy changes, update
  those source files **and** these pages.

## GitHub Pages setup

Repo **Settings → Pages → Build and deployment** → **Source: Deploy from a branch** →
**Branch: `main` / `docs`**.
