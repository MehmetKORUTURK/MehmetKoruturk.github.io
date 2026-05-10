# mehmetkoruturk.github.io

Personal academic website of **Mehmet Koruturk** — M.S. student in Electrical Engineering at **Virginia Tech**, advised by Prof. Ming Jin.

**Live site:** **<https://mehmetkoruturk.github.io>**

---

## About

I work on **reinforcement learning**, **optimization**, and **grid-interactive power systems** — specifically, on energy-management agents that are not only efficient but also safe, interpretable, and able to adapt as grid conditions, uncertainty, and disturbances evolve.

The site has five sections:

| Section | Content |
|---|---|
| **About** | Short intro and research focus |
| **Research** | Three current directions: RL benchmarking, DER coordination, post-disaster resilience |
| **Publications** | Reverse-chronological list with status badges (Accepted · Under review · In preparation · Published) |
| **CV** | Education, experience, service, awards, skills, plus a downloadable PDF |
| **Contact** | Email + social links |

---

## Tech

- Plain **HTML / CSS / JS** — no frameworks, no build step
- **GitHub Pages** for hosting (auto-deploys on push to `main`)
- Light/dark theme with system-preference detection and persistent toggle
- Fully responsive (desktop, tablet, mobile)

---

## Repository layout

```
.
├── index.html              # Main page
├── 404.html                # Not-found page
├── style.css               # Theme tokens (light/dark) + layout
├── script.js               # Theme toggle, scroll-spy, smooth scroll
├── MehmetKoruturk_CV.pdf   # Compiled CV (linked from "Download CV")
├── assets/
│   └── profile.jpg         # Profile photo
├── .nojekyll               # Tells GitHub Pages to skip Jekyll
└── robots.txt
```

The LaTeX source for the CV (`*.tex`, `*.bib`) is kept locally and is `.gitignored`; only the compiled PDF is published.

---

## Update workflow

Edit `index.html` (or `style.css` / `script.js`), then push:

```bash
git add -A
git commit -m "Update content"
git push
```

Changes go live in **~30 seconds**.

To preview locally:

```bash
python -m http.server 8000
# then open http://localhost:8000
```

---

## Contact

- **Email:** [mkoruturk@vt.edu](mailto:mkoruturk@vt.edu)
- **LinkedIn:** [mehmet-koruturk210199](https://www.linkedin.com/in/mehmet-koruturk210199/)
- **Google Scholar:** [profile](https://scholar.google.com/citations?user=0nd6K10AAAAJ&hl=en)
- **GitHub:** [@MehmetKORUTURK](https://github.com/MehmetKORUTURK)

---

<sub>© Mehmet Koruturk · Site code is free to fork.</sub>
