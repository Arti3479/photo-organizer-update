# Third-Party Licenses and Notices — macOS

Photo Organizer for macOS includes or depends on third-party software and font components.

Those components remain the property of their respective copyright holders and are governed by their own licenses.

This document is provided for attribution and license-compliance purposes.
The Photo Organizer proprietary license applies only to Photo Organizer's own code and assets and does not replace or restrict rights granted by third-party licenses.

> Platform: macOS (Apple Silicon / arm64)  
> Photo Organizer: v2.0.0

---

## Runtime Components

### Python

- Component: Python
- Version used for the current macOS build: 3.14.7
- License: Python Software Foundation License Version 2 (PSF-2.0)
- Copyright / Project: Python Software Foundation and contributors
- Official license: https://docs.python.org/3/license.html

Python may itself include software covered by additional licenses.
See the Python license and acknowledgements page above for details.

---

### CustomTkinter

- Component: CustomTkinter
- Version used for the current macOS build: 6.0.0
- License: MIT License
- Project: Tom Schimansky / CustomTkinter
- Repository: https://github.com/TomSchimansky/CustomTkinter

The applicable copyright and permission notice from the CustomTkinter distribution must be preserved where required by its license.

---

### Pillow

- Component: Pillow
- License: MIT-CMU
- Project: Python Pillow
- Repository: https://github.com/python-pillow/Pillow
- License file: https://github.com/python-pillow/Pillow/blob/main/LICENSE

Pillow may bundle or use additional image-codec libraries with their own notices and licenses.
See the Pillow distribution and its license/acknowledgement materials for the exact build being distributed.

---

### piexif

- Component: piexif
- License: MIT License
- Project: hMatoba / Piexif
- Repository: https://github.com/hMatoba/Piexif
- License file: https://github.com/hMatoba/Piexif/blob/master/LICENSE.txt

The applicable copyright and permission notice from the piexif distribution must be preserved where required by its license.

---

### tkinterdnd2 / TkinterDnD2

- Component: tkinterdnd2
- License: MIT License for the packaging project
- Project: https://github.com/pmgagne/tkinterdnd2

tkinterdnd2 packages a Tkinter wrapper together with precompiled tkDnD components.

The bundled tkDnD files and any upstream components remain subject to their own applicable notices and licenses.
When redistributing Photo Organizer, preserve the license and notice files shipped with the exact tkinterdnd2/tkDnD package used for the build.

---

### Tcl/Tk / Tkinter Runtime

Photo Organizer uses Tkinter, which relies on Tcl/Tk components distributed with Python.

- Tcl/Tk version used by the current macOS build: 9.0.x
- Python / Tkinter licensing information: https://docs.python.org/3/license.html

Any Tcl/Tk components included in the packaged application remain subject to their respective upstream licenses and notices.

---

### SUIT Typeface

- Component: SUIT
- Bundled font file: `SUIT-Variable.ttf`
- Copyright: Copyright (c) 2022, SUNN (http://sun.fo/suit)
- Reserved Font Name: SUIT
- License: SIL Open Font License 1.1 (OFL-1.1)
- Project: https://github.com/sun-typeface/SUIT

Photo Organizer bundles the unmodified SUIT font for user-interface rendering.

The SUIT font remains separately licensed under the SIL Open Font License 1.1 and is not covered by the Photo Organizer proprietary license.

The SUIT copyright notice and the full OFL 1.1 license should be kept in a separate file such as:

`SUIT_OFL.txt`

---

## Build and Packaging Tools

### PyInstaller

- Version used for the current macOS build: 6.22.3
- License: GPL 2.0 with a special exception, with certain files under Apache License 2.0
- Official license: https://pyinstaller.org/en/v6.22.3/license.html

PyInstaller's license includes a special exception intended to permit distribution of executable bundles created from your own source, subject to compliance with the licenses of bundled dependencies.

---

## Important Distribution Note

Before each public or commercial release of Photo Organizer, verify the exact versions and license files of all packages actually included in that specific build.

For compliance-sensitive distribution, especially commercial distribution or transfer of the Photo Organizer project to a company, keep copies of the exact third-party license files that correspond to the versions bundled in the application.

Recommended repository structure:

```text
LICENSE.txt
THIRD_PARTY_LICENSES.md
THIRD_PARTY_LICENSES_mac.md
licenses/
  SUIT_OFL.txt
```

Additional upstream license files may also be retained in the `licenses/` directory when required.

---

## Photo Organizer

Photo Organizer's own code and assets are governed by the repository's proprietary `LICENSE.txt` file unless explicitly stated otherwise.

Copyright © 2026 Arti3479. All rights reserved.

---

[← Windows Third-Party Licenses](THIRD_PARTY_LICENSES.md) · [README](README.md)
