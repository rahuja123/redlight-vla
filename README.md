# RedLight-VLA — Project Page

Project page for **"RedLight-VLA: Models for traffic-rule grounding and behavioral emphasis in driving policies"** (ECCV 2026, DriveX Workshop · arXiv:2608.28656).

Live site: **https://rahuja123.github.io/redlight-vla/**

## What's here
- `index.html` — self-contained project page (no build step). All CSS/JS is inline.
- `assets/og-image.png` — 1200×630 social-preview card (Open Graph / Twitter).
- `robots.txt`, `sitemap.xml`, `.nojekyll` — SEO / GitHub Pages plumbing.

## SEO built in
- `<title>` + meta description + canonical URL
- Open Graph + Twitter `summary_large_image` cards
- **Google Scholar** `citation_*` tags (title, authors, dates, PDF URL, arXiv id) so Scholar can link this page to the paper
- JSON-LD `ScholarlyArticle` structured data for Google rich results
- `robots.txt` + `sitemap.xml`

## Deploy to GitHub Pages

```bash
cd redlight-vla
git init
git add .
git commit -m "Add RedLight-VLA project page"
git branch -M main
gh repo create redlight-vla --public --source=. --remote=origin --push
# Then enable Pages: Settings → Pages → Source: "Deploy from a branch" → main / root
```

Or via the CLI once the repo exists:

```bash
gh api -X POST repos/rahuja123/redlight-vla/pages -f source.branch=main -f source.path=/
```

## After it's live (SEO follow-ups)
1. Add the site to **Google Search Console** and submit `sitemap.xml`.
2. Add the project-page URL to the paper's arXiv listing (under "other resources").
3. Validate structured data at https://search.google.com/test/rich-results.
4. Preview the social card at https://www.opengraph.xyz/ (paste the live URL).
5. When code/video/poster are ready, fill in the buttons marked `EDIT:` in `index.html`.

## Things to review / fill in
- Author **affiliations** — placeholder comment in `index.html` (search `EDIT: add author affiliations`).
- The visible hero title uses a cleaned-up phrasing; the exact arXiv title (with "Models for") is preserved in the `citation_title` and JSON-LD for correct Scholar matching.
