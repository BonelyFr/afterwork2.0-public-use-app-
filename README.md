# After Work

Plan the hours between your day and bedtime, one small block at a time. It's a web app that installs to a phone's home screen and works offline. No account, no tracking; everything is saved on the device.

## Put it on GitHub Pages
1. Create a new repository on github.com (for example `after-work`).
2. Upload everything in this folder to it (**Add file > Upload files**), including the hidden `.nojekyll` file if your browser lets you. If it doesn't, the app still works.
3. In the repo: **Settings > Pages > Build and deployment > Source: Deploy from a branch**, pick `main` and `/ (root)`, then **Save**.
4. After a minute or two it's live at `https://YOUR-USERNAME.github.io/after-work/`.

## Install it on a phone
- **iPhone:** open the link in **Safari**, tap **Share > Add to Home Screen**.
- **Android:** open it in Chrome, tap **⋮ > Install app** (or Add to Home Screen).

Tell people to **open it from the home-screen icon after installing**. On iPhone, the Safari tab and the home-screen app keep *separate* saved data, so anything entered in Safari before installing won't appear in the installed app. Use ••• > **Export backup** / **Import backup** to move data between devices or browsers.

## Updating
Edit `index.html`, commit and push; Pages republishes in a minute or two. The app checks for a newer page every time it's opened online. If you ever change `sw.js` or the icons, bump `CACHE = 'after-work-v1'` to `v2` so devices drop their old copy.

## Before you publish: fill in the placeholders
Search for these and replace them:
- `[Your Name]` in `LICENSE`
- `[Your state or country]` and `your-email@example.com` in `index.html` (the `var TERMS` block), `terms-of-use.html`, and `privacy-policy.html`

The Terms of Use (shown once on first launch, and under ••• > Terms of Use) and the Privacy Policy are plain-language templates, not legal advice.

## About protecting the code
- A **public** repo means anyone can view or fork the files; GitHub's own terms allow that regardless of the `LICENSE`. The license and in-app terms only give you a legal basis if someone copies it. Nothing technical stops copying a web app that runs in the browser.
- A **private** repo hides the code, but as far as I know GitHub Pages from a private repo needs a paid plan (Pro/Team). Check GitHub's current plans.

## Files
`index.html` (the whole app) · `sw.js` (offline) · `manifest.webmanifest` + `icon-*.png` (home-screen install) · `terms-of-use.html`, `privacy-policy.html` · `LICENSE`
