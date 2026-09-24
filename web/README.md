# Boom Bap Producer Pads — Web/PWA

The project website: <https://edensfrequency.github.io/boom-bap-producer-pads/>.
One page that introduces the plugin, lets visitors play a 16-pad drum demo
right in the browser, tours the plugin's tabs, and links to the downloads.
It can also be installed like an app (a "PWA") and keeps working offline once
visited.

Static, dependency-free PWA surface for GitHub Pages.

## What's in this folder

| Item | What it is |
|---|---|
| [index.html](index.html) | The page itself: every section's text and layout. |
| [manifest.json](manifest.json) | Tells phones and browsers how to install the site as an app (name, icons, colours). |
| [sw.js](sw.js) | The "service worker": saves the page's files so it opens instantly and works offline. Bump its asset version when files change, or returning visitors keep seeing the old ones. |
| [public/](public/README.md) | Everything the page loads: sounds, images, scripts and styles. |

## Local preview

Serve this directory with any static HTTP server. Do not open `index.html` directly as a `file://` URL if you want service-worker testing.

## GitHub Pages

Deploy the contents of `web/` as the Pages artifact. The app is intentionally relative-path based, so it works under a repository path such as:

`https://edensfrequency.github.io/boom-bap-producer-pads/`

The page currently uses remote Google Fonts. If fully offline operation is required, vendor the fonts locally and update `styles.css`.
