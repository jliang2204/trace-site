# Trace download website

Buildless static page for https://jliang2204.github.io/trace-site/.
This directory is the complete standalone `trace-site` repository. Do not upload
the parent Recorder workspace or application source to the website repository.

## Publish

Create a public `trace-site` repository under `jliang2204` and push the contents
of this directory to its `main` branch, including `.github` and `.nojekyll`.
Under Settings > Pages, select **GitHub Actions** as the build source. Run the
included Deploy Trace website workflow or push to main. GitHub provides HTTPS.

Only index.html, style.css, .nojekyll and assets/ are included in the Pages
artifact. No Node dependencies, tracking scripts, cookies or external fonts.
The arena artwork is an illustrative SVG, not an actual Trace screenshot.

## Installer

Download links use the stable Trace update-host `/download` route. That route
reads the current release publication record and redirects to the latest
available Windows installer, with caching disabled. Future app releases do not
require editing this page. The existing updater feed remains separate.

## Preview

From this directory: `python -m http.server 4173 --bind 127.0.0.1`, then open
http://127.0.0.1:4173. No build step. Check desktop and mobile widths, keyboard
navigation, native FAQ expansion and the Windows download link before publishing.

The app remains a beta; do not add unverified zero-overhead, perfect detection,
hardware compatibility or competitor performance claims.
