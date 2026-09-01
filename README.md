# Personal academic website

A simple three-page static site: About, Research, Publications & Talks.
No build tools required — just HTML, CSS, and a tiny bit of JS.

## Files to edit

- `index.html` — About page. Fill in your name, department/university,
  bio, and contact links. Add your photo (see `images/README.txt`).
- `research.html` — Research interests. Pre-filled with a draft based on
  your research statement — edit freely.
- `publications.html` — Publications & presentations. Replace the
  placeholder `[Paper title]` / `[Talk title]` entries with your own.
- `css/style.css` — Shared styling. You shouldn't need to touch this
  unless you want to change colors/fonts/layout.
- `images/photo.jpg` — Add your headshot here (instructions in
  `images/README.txt`).
- `cv.pdf` — Add your CV here (referenced from the About page's contact
  list; remove that link if you'd rather not host your CV directly).

Every `[bracketed placeholder]` in the HTML is something to replace with
your own text. Search for `[` in each file to find them all.

## Publishing with GitHub Pages

1. Create a new GitHub repository — for a personal site, name it
   `yourusername.github.io` (replace `yourusername` with your actual
   GitHub username). This exact naming makes GitHub host it at
   `https://yourusername.github.io` automatically. (Any other repo name
   also works, just at `https://yourusername.github.io/repo-name`.)
2. Copy all the files in this folder into that repository (keep the
   folder structure: `css/`, `images/`, and the three `.html` files at
   the top level).
3. Commit and push:
   ```
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/yourusername/yourusername.github.io.git
   git push -u origin main
   ```
4. On GitHub, go to the repository's **Settings → Pages**. Under
   "Build and deployment," set Source to "Deploy from a branch," branch
   `main`, folder `/ (root)`. Save.
5. Wait a minute or two, then visit `https://yourusername.github.io` (or
   the repo-name URL if you used a different repo name).

Any time you push new commits to `main`, the live site updates
automatically within a minute or so.

## Adding this to your resume

Once it's live, add the URL under your contact info or a "Websites" /
"Links" line on your CV — e.g. `yourusername.github.io`.
