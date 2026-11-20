# Pinwheel for Windows

Pinwheel opens a wheel of conversions, tools and file actions around the pointer while you drag files in File
Explorer. Press **Ctrl** mid-drag (or hold it as the drag starts), point at **Convert**, **Tools** or **Actions**, and
drop on an option. Results are saved beside the originals, and everything runs on your PC: no uploads, no account.

- **Convert** between 46 formats: images, audio, video, documents, ebooks, spreadsheets, slides, PDFs and archives.
- **27 tools**: compress, edit metadata, edit, annotate, crop, redact and upscale photos, trim, split, crop, speed up
  and redact videos, trim and normalize audio, split, merge and organize PDFs, and more.
- **File actions**: share, copy, move, copy the path, open a terminal there, and Float (a shelf that keeps files at
  hand).

## Download

**[Download Pinwheel for Windows](https://github.com/Emin-Emini/pinwheel-windows-releases/releases/latest/download/Pinwheel-win-x64-setup.exe)**
(the installer, for most PCs). Every version is on **[Releases](https://github.com/Emin-Emini/pinwheel-windows-releases/releases/latest)**.
Pick the one for your PC (Settings → System → About → System type):

| Your PC | Installer | Portable zip |
|---|---|---|
| x64-based processor (most PCs: Intel and AMD) | [`Pinwheel-win-x64-setup.exe`](https://github.com/Emin-Emini/pinwheel-windows-releases/releases/latest/download/Pinwheel-win-x64-setup.exe) | [`Pinwheel-win-x64.zip`](https://github.com/Emin-Emini/pinwheel-windows-releases/releases/latest/download/Pinwheel-win-x64.zip) |
| ARM-based processor (Snapdragon and other Windows on Arm PCs) | [`Pinwheel-win-arm64-setup.exe`](https://github.com/Emin-Emini/pinwheel-windows-releases/releases/latest/download/Pinwheel-win-arm64-setup.exe) | [`Pinwheel-win-arm64.zip`](https://github.com/Emin-Emini/pinwheel-windows-releases/releases/latest/download/Pinwheel-win-arm64.zip) |

The x64 installer also runs on ARM PCs with Windows 11; the ARM one is faster there.

**Needs** Windows 10 22H2 or Windows 11. HEIC output needs the HEIF and HEVC Video Extensions from the Microsoft Store.
Enhanced upscaling needs the Microsoft Visual C++ Redistributable, and Upscale Image links to it when it's missing.

## Install

1. Open **Pinwheel-win-x64-setup.exe**. If Windows says "Windows protected your PC", choose **More info** →
   **Run anyway**. It installs for you only and doesn't need administrator rights.
2. Choose whether Pinwheel launches when you sign in and appears in File Explorer's **Send to** menu, then **Install**.
3. Pinwheel sits in the notification area by the clock. Getting Started opens the first time.

To update, run the newer installer: it replaces the old version and keeps your settings. **To remove Pinwheel:**
Settings → Apps → Installed apps → Pinwheel → Uninstall.

> **Unsigned for now.** Pinwheel isn't code-signed yet. That's why Windows warns about it, and why **Smart App
> Control** blocks it outright: while Smart App Control is on (Windows Security → App & browser control), Pinwheel
> can't run on that PC.

### Portable zip, without installing

Right-click the zip → **Properties** → tick **Unblock** → OK, then **Extract All…**, keep the **Pinwheel** folder
somewhere it can stay, and open **Pinwheel.exe**. To remove it: turn off Launch at startup in Settings, quit Pinwheel
from its tray icon (**Quit Pinwheel**), then delete the folder, `%APPDATA%\Pinwheel` and `%LOCALAPPDATA%\Pinwheel`.

## Problems, ideas and questions

Please **[open an issue](https://github.com/Emin-Emini/pinwheel-windows-releases/issues/new/choose)**. This is
Pinwheel's first Windows version, so every report helps. Say which Windows version and PC you have, what you did, and
what happened. Pinwheel's log is in `%LOCALAPPDATA%\Pinwheel\Logs`; attaching the day's file helps a lot. It holds file
names and folder paths, never the contents of your files, so check it before you share it.

## Licences

Pinwheel for Windows is © 2026 Emin Emini. It includes third-party components under their own licences, among them
FFmpeg (LGPL 3.0) and ImageMagick's LGPL libraries. The installer shows the licence, and each download holds `LICENSE.txt`, `THIRD-PARTY-NOTICES.txt` and a
`licenses` folder. The complete source of the copyleft components is at
[pinwheel-third-party-sources](https://github.com/Emin-Emini/pinwheel-third-party-sources). Pinwheel's own source code
isn't published here.
