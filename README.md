# ClipStudio — JIAN PLAY STUDIOS

## Package contents
- `index.html` — the original ClipStudio single-file app, with install/offline registration added.
- `hero.jpg` — the original artwork.
- `manifest.webmanifest` — install metadata for supported browsers.
- `sw.js` — same-origin app-shell cache for offline reopening after the first successful load.

## Deploy / update
1. Extract this ZIP.
2. Upload all four files to the root of the existing `jian012209-oss/ClipStudio` repository, replacing the old `index.html` and keeping `hero.jpg`.
3. Commit the changes and wait for GitHub Pages / your existing hosting deployment to finish.
4. Open the deployed site once while online. The service worker then caches the app shell.
5. On Android Chrome, use the browser menu and choose **Install app** or **Add to Home screen** if offered.

## Notes
- Keep the files together in the same folder/root; the app expects relative paths.
- Offline support caches the app shell only. Imported media and project data remain subject to the browser's existing local storage and device limits.
- This package preserves the existing ClipStudio UI and editor code. It does not claim to add a server, cloud sync, or new professional rendering codecs.
- The editor's actual export capability depends on browser/device encoder support. Test exports on the target Android device before distributing a release.
- Admin signing keys and local project data are device/browser-local; do not treat this static package as a secure centralized licensing backend.
