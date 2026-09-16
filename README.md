**English** | [한국어](README_KR.md)
# Photo Organizer

Photo Organizer is a Windows photo management application that supports film photo metadata management, LUT application for digital photos, automatic folder organization, RAW matching, file timestamp management, duplicate file detection, and more.

Current version: **v2.0.0**

---

## Key Features

### Film Photo Management

- Import multiple photos at once
- Change photo order
- Apply sequential capture times
- Enter exact capture times manually
- Write capture times to EXIF metadata
- Record camera manufacturer / body / lens information
- Record film stock information
- Synchronize Windows file creation / modification dates

### Digital Photo LUT

- Supports JPEG / PNG / TIFF
- Supports `.cube` LUT files
- Adjust LUT strength from 0–100%
- Side-by-side preview of original and LUT-applied images
- Navigate through multiple photos using Previous / Next
- LUT library management
- Export as JPG / PNG / TIFF
- Keep the original image format when exporting

The `Save` function does not overwrite the original file. Instead, it creates a new `_LUT` file in the same folder as the original.

Example:

```text
IMG_0001.jpg
IMG_0001_LUT.jpg
```

`Save As` allows you to manually choose the save location and file name.

---

## Folder Sorting

Photos can be automatically organized by:

- File extension
- Capture date
- Camera model
- Lens

Photos inside previously sorted folders can also be reorganized recursively.

If a file with the same name already exists, you can choose one of the following options:

- Auto Rename
- Skip
- Overwrite

> The Folder Sorting feature physically moves files. Backing up important photos before sorting is recommended.

---

## JPEG → RAW Matching

Photo Organizer can find RAW files with the same file name as JPEG photos and automatically copy the matching originals.

Examples of supported RAW formats:

- CR3
- CR2
- NEF
- ARW
- RAF
- ORF
- RW2
- DNG

---

## File Timestamp Management

Sequential capture times can be applied to multiple photos at once.

Windows file creation and modification dates can also be updated when needed.

---

## Duplicate File Detection

Photo Organizer uses SHA-256 to identify identical files.

For improved performance, files are first grouped by file size, and SHA-256 hashes are calculated only for files that are potential duplicates.

---

## Supported Languages

Photo Organizer supports the following languages:

- 한국어
- English
- 日本語
- 简体中文
- Français
- Español
- Deutsch
- Русский

The application name **Photo Organizer** remains the same in every language.

---

## Installation

1. Go to the GitHub **Releases** page.
2. Download the latest installer.
3. Run the installer.
4. Launch Photo Organizer after installation is complete.

For general users, the following installer is recommended:

```text
PhotoOrganizer_Setup_v2.0.0.exe
```

The standalone `PhotoOrganizer.exe` is provided primarily for the application's automatic update system.

---

## Automatic Updates

Photo Organizer supports automatic update checking and installation.

Update process:

1. Check for a newer version
2. Download the new application
3. Verify file integrity using SHA-256
4. Launch the updater
5. Close the currently running application
6. Safely replace the application with the new version
7. Automatically restart the updated version

If an update fails, the existing application remains unchanged.

---

## Database Updates

The following databases can be updated separately from the main application:

- Camera database
- Film database
- Fixed-lens camera database

---

## LUT Library

LUT files are stored by default in:

```text
Documents\Photo Organizer\LUTs
```

You can create subfolders to organize your LUT files. Photo Organizer automatically searches LUT files inside subfolders as well.

---

## Offline Use

Photo Organizer includes built-in camera and film databases, allowing its main features to work without an internet connection.

An internet connection may be required for:

- Application updates
- Database updates

---

## System Requirements

- Windows 10 / Windows 11
- 64-bit Windows recommended

---

## Download

The latest version can be downloaded from GitHub Releases.

**Release:**  
https://github.com/Arti3479/photo-organizer-update/releases

---

## Feedback & Data Requests

For bug reports, camera / film database addition requests, or suggestions for improvements, use:

**Help → Feedback & Data Request**

inside Photo Organizer.

---

## Important Notes

- Backing up important photos before processing is recommended.
- The Folder Sorting feature physically moves files.
- The File Timestamp feature may modify Windows file information and EXIF metadata.
- LUT saving is designed to preserve the original image, but keeping separate backups of important original photos is still recommended.

---

## Version

### v2.0.0

First official release of Photo Organizer.

Major changes:

- Improved film photo metadata and capture time management
- Added LUT application and export features for digital photos
- Added Save and Save As functionality
- Improved recursive folder sorting and file conflict handling
- Added multilingual UI support
- Improved memory management and application stability
- Added automatic update support

---

## Development

Photo Organizer is developed using Python.

Main technologies:

- Python
- Tkinter
- CustomTkinter
- Pillow
- piexif
- tkinterdnd2
- PyInstaller
- Inno Setup

---
## License

Photo Organizer is proprietary freeware.

The software is free for personal, non-commercial use.  
Redistribution, sale, commercial use, and distribution of modified versions are not permitted without prior written permission from the copyright holder.

All copyrights and intellectual property rights remain with the copyright holder.

See [LICENSE](LICENSE) for the full license terms.

© 2026 Arti3479
