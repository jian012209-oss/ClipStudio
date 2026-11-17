# ClipStudio — Android package

A mobile-first editing prototype combining a CapCut-inspired basic workflow with Alight Motion-inspired layer and motion-graphics controls.

## Included
- Responsive dark purple/blue ClipStudio interface
- Basic and Pro workspace modes
- Local project save/list/open/delete
- Import video, image, and audio assets
- Multi-lane timeline (video/image, text/graphics, audio)
- Select, duplicate, delete, split, and arrange imported assets
- Preview for selected video/image assets
- Text and shape layers
- Inspector controls for duration, start, opacity, scale, rotation, brightness, contrast, saturation
- Effect presets and basic preview filters
- Pro activation-code generator in Admin Studio
- GitHub Actions workflow to build a debug APK

## Build APK with GitHub
1. Upload the contents of this folder to the root of your GitHub repository, including the hidden `.github` folder.
2. Open **Actions** in the repository.
3. Run **Build ClipStudio Android APK**.
4. When successful, download the `ClipStudio-debug-apk` artifact from the workflow run.

## Current limitations
This is a functional starter editor, not a feature-equivalent replacement for CapCut or Alight Motion. Full multi-track compositing/export to MP4, frame-accurate audio mixing, real vector/mask rendering, graph interpolation, and advanced GPU effects still require a native rendering engine and additional implementation. The Export button currently does not render a complete composed MP4.

The admin password check is a client-side gate intended only for personal local use. It is not secure against someone inspecting the app files. Pro activation and projects are local to this device/browser; generated codes are not remotely transferable.

## App identity
- App name: ClipStudio
- Package ID: com.jianplaystudios.clipstudio
- Studio: JIAN PLAY STUDIOS
