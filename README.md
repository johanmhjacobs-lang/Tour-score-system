# The Tour — installable app setup (GitHub Pages)

This folder is a ready-to-host installable web app. Once it's on GitHub Pages,
Chrome on Android will offer a real **"Install app"** prompt.

## One-time setup

1. Go to [github.com/new](https://github.com/new) and create a new repository.
   - Name it anything, e.g. `the-tour` or `aic-cricket-tour`.
   - Set it to **Public** (GitHub Pages on a free account needs a public repo).
   - Don't add a README/gitignore/license — leave it empty.

2. Upload the files in this folder to that repository:
   - On the repo's page, click **"Add file" → "Upload files"**.
   - Drag in all 7 files from this folder: `index.html`, `manifest.json`, `sw.js`,
     `icon-192.png`, `icon-512.png`, `icon-512-maskable.png`, and this `README.md`.
   - Click **"Commit changes"**.

3. Turn on GitHub Pages:
   - In the repo, go to **Settings → Pages**.
   - Under "Build and deployment", set **Source** to "Deploy from a branch".
   - Set **Branch** to `main` (or `master`) and folder to `/ (root)`.
   - Click **Save**.
   - GitHub will give you a URL like `https://<your-username>.github.io/<repo-name>/`
     — it can take a minute or two to go live the first time.

## Installing it on Android

1. Open that URL in **Chrome** on your Android phone.
2. Tap the **⋮** menu → you should now see **"Install app"** (not just "Add to
   Home screen") — tap it.
3. It installs with its own icon, opens full-screen with no browser bar, and
   works offline once you've opened it at least once.

## Installing it on iPhone

Safari doesn't use the install prompt the same way — open the URL in **Safari**,
tap **Share → Add to Home Screen**. It'll behave the same way (full-screen,
own icon).

## Making changes later

Whenever the scoring rules, roster, or branding need updating, come back to
Claude with the change you want, and re-upload the new `index.html` (or
whichever files changed) to the same GitHub repo — GitHub Pages picks up the
new version automatically within a minute or two, and everyone who already
installed the app will get the update the next time they open it (thanks to
the service worker checking for a new version).
