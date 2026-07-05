# Nikita Pardeshi — Resume Site

A single-page personal resume site (HTML/CSS/JS, no build step) ready to host on GitHub Pages.

Live URL (after setup): `https://<your-username>.github.io/resume/`

## Files

- `index.html` — the page structure and content
- `styles.css` — styling (fonts, layout, colors, animations)
- `script.js` — scroll-reveal animation
- `favicon.svg` — site icon (NP monogram)
- `Nikita_Pardeshi_Resume.pdf` — downloadable resume linked from the "Resume" section

## Run locally

Just open `index.html` in a browser. Or serve it:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to GitHub Pages

1. Create a public repo named `resume` under your GitHub account.
2. Push these files to the `main` branch:

   ```bash
   cd nikita-resume
   git init
   git add .
   git commit -m "Add resume site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/resume.git
   git push -u origin main
   ```

3. In the repo, go to **Settings → Pages**:
   - Source: **Deploy from a branch**
   - Branch: `main`
   - Folder: `/ (root)`
4. Wait a minute, then open `https://<your-username>.github.io/resume/`.

## Customize

- **Text/content:** edit the sections inside `index.html`.
- **Colors:** change the `--accent` and `--accent-2` variables at the top of `styles.css`.
- **Resume PDF:** replace `Nikita_Pardeshi_Resume.pdf` (keep the same filename, or update the link in `index.html`).

## Credit

Structure and visual style adapted from the layout at
[github.com/khire12/resume](https://github.com/khire12/resume).
