# Lucas Kersten — academic website (version 8)

A lightweight, single-page academic website. Built with plain HTML, CSS, and minimal JavaScript. No dependencies, build tools, or accounts required to run it locally.

## Run locally

**Simplest:** double-click `index.html` to open it in your browser.

**Optional local server:** from this folder, run:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000 . Stop the server with Ctrl+C.

## Edit content

- `index.html` — all text, publications, teaching, talks, and links.
- `style.css` — colors, typography, spacing, and mobile layout.
- `script.js` — mobile menu.
- `assets/lucas-kersten.jpg` — your portrait photo, displayed in the hero section. Replace this file to update the photo.
- `assets/cv.pdf` — replace with your updated CV (keep the filename).
- `assets/eigenfunction.svg` — decorative illustration; regenerate using `python generate_illustration.py` if you have NumPy and Matplotlib installed.

### Add a publication

Copy an existing `<li class="publication">...</li>` inside the `publication-list` in `index.html`. Update title, authors, year, link, and the displayed number. Use real publications only.

### Add teaching details

Edit the `<details class="teaching-item">` blocks in `index.html`. Each course now has its own responsibility paragraph. The initial text **"Add course-specific responsibilities here"** is deliberately a placeholder: the CV gives responsibilities collectively for each institution, not by course. Replace these placeholders with accurate course-specific descriptions. Both institutions are collapsed by default.

## Publish on GitHub Pages (when ready)

1. Create a GitHub account, if you do not have one.
2. Create a **public** repository named `YOUR-USERNAME.github.io` (replace with your actual GitHub username).
3. Upload all files and the `assets` folder to the repository root, or push using Git.
4. In **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/ (root)`, and save.
5. Wait for deployment and visit `https://YOUR-USERNAME.github.io/`.

When the public URL is known, consider adding a canonical URL, Open Graph URL, `robots.txt`, and a `sitemap.xml`. Google Search Console can then be configured for indexing monitoring. Search results are not guaranteed.

## Content notes

- Academic details are based on the supplied CV. Only the real preprint `arXiv:2609.16746` is included.
- The December 2026 Stuttgart presentation is marked **planned**, as in the CV. Update or remove it after the event.
- Individual teaching semesters are not specified in the CV, so the site lists institution-level periods rather than inventing semesters.
- The SVG uses contours of `sin(2πx) sin(2πy)`, a Dirichlet eigenfunction on the unit square. It is a decorative mathematical example, not a visualization of Lucas's research results.
- No analytics, tracking cookies, external fonts, or JavaScript libraries are used.


## Version 3 changes
- Teaching is grouped by university and course, without years or semesters. Each course has its own responsibility placeholder to edit.
- The OTQP 2026 flash talk now explicitly links to Publication 01.
- Academic Activities uses text headings instead of ambiguous decorative pictograms.

## Version 4 changes
- Both teaching panels start collapsed; click an institution to expand its course-specific entries.
- The OTQP 2026 flash talk refers to **Publication 01**, which links to the matching publication entry on this page (not directly to arXiv).
- The publication entry is highlighted when reached by its internal link.
- Further research illustrations are intentionally not added yet, pending a visual choice.

## Version 5 changes
- Research overview now sits directly below the Research heading.
- The last course in each teaching group has the same bottom divider as the other courses.
- No additional research illustrations were added.

## Version 6 changes
- The Research introduction now sits to the right of the heading, aligned with the About section and using the same body font and color.

## Version 7 teaching update

Teaching responsibilities are now listed individually for each course. The separate Python Programming course entry was removed; Python computer labs are included under Single-Variable Calculus. Teaching panels remain collapsed by default.

### Version 9 layout adjustment

The portrait is larger and the mathematical illustration smaller in the hero section, with responsive sizing for tablet and mobile. All other content is unchanged.
