# Mehmet Koruturk — Personal Website

Static personal site for **Mehmet Koruturk**, M.S. student in Electrical Engineering at Virginia Tech.
No build step. No frameworks. Pure HTML / CSS / JS — drop on GitHub Pages and it works.

## Files

```
website/
├── index.html              # Main page (about, research, publications, CV, news, contact)
├── 404.html                # Not-found page
├── style.css               # Theme tokens (light/dark) + layout
├── script.js               # Theme toggle, scroll-spy, smooth scroll
├── MehmetKoruturk_CV.pdf   # Linked from "Download CV" / "Full CV (PDF)"
├── .nojekyll               # Tells GitHub Pages: don't run Jekyll
├── robots.txt              # SEO
└── assets/                 # For profile.jpg, etc.
```

---

## Deploy to GitHub Pages

### Option A — `mkoruturk.github.io` (root site, recommended)

1. Create a new public repo named **exactly** `mkoruturk.github.io`
   (replace with your real GitHub username if different).
2. From this folder:
   ```bash
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/mkoruturk/mkoruturk.github.io.git
   git push -u origin main
   ```
3. In the repo on GitHub: **Settings → Pages → Source = `Deploy from a branch`**, branch = `main`, folder = `/ (root)`. Save.
4. Wait ~1 minute. Visit `https://mkoruturk.github.io`.

### Option B — Project page

If you'd rather host this from a regular repo (e.g. `personal-site`):

1. Push the contents to that repo.
2. **Settings → Pages → Source = `main` / `(root)`**.
3. URL becomes `https://USERNAME.github.io/personal-site/`.

---

## Customize

### Add your photo

1. Drop a square photo at `assets/profile.jpg` (≥ 400×400 px).
2. In `index.html` find the comment `<!-- Replace with: <img ... /> -->`,
   uncomment that line, and delete the `<div class="photo-placeholder">MK</div>` block.

### Update GitHub / Scholar URLs

In `index.html`, the social icons currently point to placeholder roots:

| Icon          | Replace                                    |
|---------------|--------------------------------------------|
| GitHub        | `https://github.com/`                      |
| Google Scholar | `https://scholar.google.com/citations?user=&hl=en` (paste your real Scholar profile URL once you have one) |

LinkedIn (`mehmet-koruturk210199`), email (`mkoruturk@vt.edu`), and phone are already filled from your CV.

### Update the CV

Replace `MehmetKoruturk_CV.pdf` with a fresher copy whenever you update your CV.
Both buttons ("Download CV", "Full CV (PDF)") point to that filename.

### Change accent color

In `style.css`, edit the `--accent` variables. Currently:
- Light: VT-style maroon `#8b1a1a`
- Dark: amber `#f59e0b`

### Add news entries

Edit the `<aside class="news">` block in `index.html`. Each `<li>` is one entry —
short and dated. Newest at the top.

---

## Local preview

```bash
# Python 3
python -m http.server 8000

# or Node
npx serve .
```

Then visit `http://localhost:8000`.

---

## License

Content (text, CV) © Mehmet Koruturk. Site code is free to fork.
