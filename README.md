# ClipStudio

A responsive dark-themed video-editing and motion-graphics UI prototype.

## Included
- Home, projects, editor, effects/assets, Pro membership, and Admin Studio screens
- Fake login/sign-up interface and guest access
- Basic/Pro mode presentation
- Local demo activation-code generator and one-time redemption
- Browser media preview, playback, seeking, speed, volume, filters, and text overlay
- Project metadata saved in browser localStorage
- GitHub Actions workflow for GitHub Pages

## Important prototype limits
This is a front-end prototype, not a finished professional video-rendering application.
MP4 rendering, a full multi-track editing engine, keyframe animation, cloud sync, and
secure cross-device activation are not implemented.

The activation-code screen and Admin Studio are local demo logic only. Codes generated
in one browser are not shared with other devices. Before distributing real Pro codes,
connect a secure backend that stores hashed codes and enforces single-use redemption,
expiry, and revocation. Do not put admin secrets in this static site.

## Publish
1. In GitHub, open **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to **GitHub Actions**.
3. Push this repository to `main`; the workflow deploys the site.
4. The site URL will be `https://jian012209-oss.github.io/ClipStudio/`.
