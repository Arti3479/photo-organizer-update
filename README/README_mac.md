# Photo Organizer — macOS

[Windows · English](../README.md) | [Windows · 한국어](README_KR.md) | **macOS · English** | [macOS · 한국어](README_mac_KR.md)

Photo Organizer is a desktop application for organizing film and digital photos, managing metadata and file times, applying LUTs, sorting folders, and performing utility tasks.

> Current macOS build: **v2.0.0**  
> Architecture: **Apple Silicon (arm64)**

---

## Main Features

### Film Photos
- Reorder photos by buttons or mouse drag
- Apply sequential or exact capture times
- Write EXIF `DateTimeOriginal`
- Camera / lens / film metadata support
- Fixed-lens camera fallback database
- Batch metadata application

### Digital Photos
- Apply `.cube` LUT files
- LUT strength control
- Original / applied preview
- Previous / next image navigation
- Save to sibling `*_LUT` folder
- Save As support
- JPEG / PNG / TIFF output options
- LUT library stored in `Documents/Photo Organizer/LUTs`

### Folder Sorting
- Sort files into folders
- RAW matching support for related files
- Collision-safe file handling

### File Time
- Batch-edit file date and time information

### Tools
- SHA-256 duplicate-file checking
- Reset / About utilities

### Languages
- 한국어
- English
- 日本語
- 简体中文
- Français
- Español
- Deutsch
- Русский

---

## macOS Requirements

- macOS on **Apple Silicon**
- M1 / M2 / M3 / M4 series supported by the current arm64 build
- Intel Mac build is not currently provided

The current macOS build uses:

- Python 3.14.7
- Tcl/Tk 9.0.x
- CustomTkinter 6.0.0
- Pillow
- piexif
- tkinterdnd2
- SUIT typeface

---

## Installation

When a public macOS build is provided:

1. Download the macOS arm64 ZIP file.
2. Extract the ZIP.
3. Move `Photo Organizer.app` to the `Applications` folder.
4. Open the app.

### Gatekeeper Notice

The current free macOS build uses **ad-hoc code signing** and is not notarized with an Apple Developer ID.

On first launch, macOS may block the app.

If that happens:

1. Control-click or right-click `Photo Organizer.app`.
2. Select **Open**.
3. Select **Open** again.

Depending on the macOS version, you may also need to allow the app in:

`System Settings → Privacy & Security`

---

## Code Signing

The macOS v2.0.0 arm64 build has been verified locally with:

```bash
codesign --verify --deep --strict
```

The build passes code-signature integrity verification.

Because the app is not signed with an Apple Developer ID and has not been notarized by Apple, Gatekeeper may still display a warning when the app is downloaded on another Mac.

---

## Third-Party Licenses

- [macOS Third-Party Licenses](../THIRD_PARTY_LICENSES_mac.md)
- [SUIT Open Font License](../licenses/SUIT_OFL.txt)
- [Photo Organizer License](../LICENSE.txt)

---

## License

Photo Organizer is proprietary freeware.

Personal, non-commercial use is permitted free of charge under the terms of the project license.

Commercial use, redistribution, integration into a commercial product or service, and other rights not expressly granted require separate permission.

See:

[LICENSE.txt](../LICENSE.txt)

---

## Copyright

Copyright © 2026 Arti3479. All rights reserved.
