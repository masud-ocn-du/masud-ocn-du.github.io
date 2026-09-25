# Md Masud-Ul-Alam — Researcher Website

A fast, responsive, accessible static website designed for GitHub Pages. It uses plain HTML, CSS, and JavaScript, so no build tools or paid hosting are required.

## Publish it on GitHub

1. Sign in to GitHub and create a public repository named `YOUR-USERNAME.github.io`.
2. Download and unzip this package.
3. Upload **the contents inside the folder** (`index.html`, `assets`, etc.) to the repository root. Do not upload only the outer folder.
4. Commit the files to the `main` branch.
5. Open **Settings → Pages**.
6. Under **Build and deployment**, choose **Deploy from a branch**.
7. Select `main`, choose `/ (root)`, and click **Save**.
8. Your site address will be `https://YOUR-USERNAME.github.io/`.

## Important edits before publishing

Search `index.html` for these items:

- `mm59115@uga.edu`: verify this is the email you want public.
- Google Scholar, ResearchGate, and UGA profile links: already inserted.
- `243`, `7`, and `6`: Scholar citation metrics, h-index, and i10-index. Update them periodically.
- Biography, research, teaching, and publications: review every statement.
- Publication records: verify final author lists, issue/page details, and DOI links if you add them.

## Add your photograph

1. Put a square or portrait image at `assets/profile.jpg`.
2. In `index.html`, replace:

```html
<div class="portrait" aria-hidden="true">MM</div>
```

with:

```html
<img class="portrait" src="assets/profile.jpg" alt="Portrait of Md Masud-Ul-Alam">
```

The existing CSS will size it. Add `object-fit: cover;` to `.portrait` in `assets/style.css` if needed.

## Add a CV button

1. Put the PDF at `assets/Md-Masud-Ul-Alam-CV.pdf`.
2. Add this link inside the hero `<div class="actions">` block:

```html
<a class="button secondary" href="assets/Md-Masud-Ul-Alam-CV.pdf" target="_blank">Download CV</a>
```

## Customize the design

At the top of `assets/style.css`, edit the variables in `:root`. For example, `--sea` controls the main accent color and `--ink` controls the dark text/background color. Comments in each file explain the major sections.

## Suggested maintenance

- Update publications and metrics every 3–6 months.
- Compress photographs before uploading.
- Do not place private information, unpublished data, or copyrighted PDFs in a public repository unless you have permission.
- Test links after every update.

## File structure

```text
index.html
assets/
  style.css
  script.js
README.md
.nojekyll
```
