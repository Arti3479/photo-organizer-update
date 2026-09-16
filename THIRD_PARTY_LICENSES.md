# Third-Party Licenses and Notices

Photo Organizer includes or depends on third-party software.  
Those components remain the property of their respective copyright holders and are governed by their own licenses.

This document is provided for attribution and license-compliance purposes.  
The Photo Organizer proprietary license applies only to Photo Organizer's own code and assets and does not replace or restrict rights granted by third-party licenses.

---

## Runtime Components

### Python

- Component: Python
- Version used for the current Windows build: 3.14.7
- License: Python Software Foundation License Version 2 (PSF-2.0)
- Copyright / Project: Python Software Foundation and contributors
- Official license:
  https://docs.python.org/3/license.html

Python may itself include software covered by additional licenses. See the Python license and acknowledgements page above for details.

---

### CustomTkinter

- Component: CustomTkinter
- License: MIT License
- Project: Tom Schimansky / CustomTkinter
- Repository:
  https://github.com/TomSchimansky/CustomTkinter

The applicable copyright and permission notice from the CustomTkinter distribution must be preserved where required by its license.

---

### Pillow

- Component: Pillow
- License: MIT-CMU
- Project: Python Pillow
- Repository:
  https://github.com/python-pillow/Pillow
- License file:
  https://github.com/python-pillow/Pillow/blob/main/LICENSE

Pillow may bundle or use additional image-codec libraries with their own notices and licenses.  
See the Pillow distribution and its license/acknowledgement materials for the exact build being distributed.

---

### piexif

- Component: piexif
- License: MIT License
- Project: hMatoba / Piexif
- Repository:
  https://github.com/hMatoba/Piexif
- License file:
  https://github.com/hMatoba/Piexif/blob/master/LICENSE.txt

The applicable copyright and permission notice from the piexif distribution must be preserved where required by its license.

---

### tkinterdnd2 / TkinterDnD2

- Component: tkinterdnd2
- License: MIT License for the packaging project
- Project:
  https://github.com/pmgagne/tkinterdnd2

tkinterdnd2 packages a Tkinter wrapper together with precompiled tkDnD components.  
The bundled tkDnD files and any upstream components remain subject to their own applicable notices and licenses.  
When redistributing Photo Organizer, preserve the license and notice files shipped with the exact tkinterdnd2/tkDnD package used for the build.

---

### Tcl/Tk / Tkinter Runtime

Photo Organizer uses Tkinter, which relies on Tcl/Tk components distributed with Python.

- Python / Tkinter licensing information:
  https://docs.python.org/3/license.html

Any Tcl/Tk components included in the packaged application remain subject to their respective upstream licenses and notices.

---

## Build and Packaging Tools

The following tools are used to build or package Photo Organizer.  
Their licenses do not change the proprietary license of Photo Organizer itself, subject to compliance with the licenses of distributed dependencies.

### PyInstaller

- Version used for the current Windows build: 6.22.3
- License: GPL 2.0 with a special exception, with certain files under Apache License 2.0
- Official license:
  https://pyinstaller.org/en/v6.22.3/license.html

PyInstaller's official license documentation states that executable bundles created from your own source may be distributed under the license of your choice, provided that the licenses of bundled dependencies are respected.

---

### Inno Setup

- Component: Inno Setup
- Project:
  https://jrsoftware.org/isinfo.php
- License / purchase information:
  https://jrsoftware.org/ishelp/topic_purchase.htm

Inno Setup is used to create the Windows installer for Photo Organizer.  
Its own license and commercial-use terms apply to use of the Inno Setup compiler and development tools.

---

## Important Distribution Note

Before each public or commercial release of Photo Organizer, the developer should verify the exact versions and license files of all packages included in that specific build.

For compliance-sensitive distribution, especially commercial distribution or transfer of the Photo Organizer project to a company, keep copies of the exact third-party license files that correspond to the versions actually bundled in the executable.

A recommended repository structure is:

```text
LICENSE
THIRD_PARTY_LICENSES.md
licenses/
  Python-LICENSE.txt
  CustomTkinter-LICENSE.txt
  Pillow-LICENSE.txt
  piexif-LICENSE.txt
  tkinterdnd2-LICENSE.txt
  tkdnd-LICENSE.txt
```

Only include license files that correspond to components actually distributed with the build.

---

## Photo Organizer

Photo Organizer's own code and assets are governed by the repository's proprietary `LICENSE` file unless explicitly stated otherwise.

Copyright Â© 2026 Arti3479. All rights reserved.

