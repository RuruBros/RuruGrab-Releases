# RuruGrab

[![Latest Release](https://img.shields.io/github/v/release/RuruBros/RuruGrab-Releases)](../../releases/latest)
![Platform](https://img.shields.io/badge/platform-Windows%2011%20x64%20%7C%20macOS%20Apple%20Silicon-blue)
![Status](https://img.shields.io/badge/status-beta-orange)
![i18n](https://img.shields.io/badge/i18n-KO%20%7C%20EN%20%7C%20JA%20%7C%20ZH-green)

**Language:** [English](README.md) | [한국어](README.ko-KR.md) | [日本語](README.ja.md) | [简体中文](README.zh-CN.md)

RuruGrab is a local-first desktop app for collecting, organizing, and finding things again.

It brings together file management, batch rename, duplicate detection, web text extraction, encrypted vault notes, and catalog-style multi-drive browsing in one workspace.

## Features

- **File Management**
  - organize files by rules
  - batch rename files
  - find duplicate files

- **OneSpace**
  - browse files across multiple drives in one unified view
  - work with scattered files more comfortably

- **Web Capture**
  - extract text from web pages into Markdown
  - save and search captured content later

- **Vault**
  - keep private notes encrypted on your machine
  - protected by a master password

- **Browser Companion**
  - works with Chrome and Edge
  - sends supported content into the desktop app

## Installation

### Desktop App
1. Open the [Releases](../../releases/latest) page.
2. Download the package for your platform:
   - Windows: `RuruGrab_*-setup.exe`
   - macOS Apple Silicon: `RuruGrab_*.dmg`
3. Install and launch RuruGrab.

For macOS, the app may require the normal first-launch approval flow for apps downloaded outside the Mac App Store.

### Browser Extension
1. Open `chrome://extensions/` or `edge://extensions/`
2. Enable **Developer mode**
3. Click **Load unpacked**
4. Select the `extension` folder inside the installed RuruGrab directory.

Example Windows path:

```text
C:\Users\<YourUserName>\AppData\Local\RuruGrab
```

Example macOS app bundle path:

```text
/Applications/RuruGrab.app/Contents/Resources/extension
```

## Bundled Tools

RuruGrab includes the external command-line tools it needs for supported download and media workflows.

- `yt-dlp`
- `gallery-dl`
- `ffmpeg`
- `ffprobe`
- `fpcalc` where supported

macOS release builds use Apple Silicon sidecar names such as `gallery-dl-aarch64-apple-darwin`. The macOS `gallery-dl` sidecar is built from Codeberg source with PyInstaller because upstream release assets are Windows/Linux executables.

Release maintainers can refresh bundled tools from the application repository with:

```bash
cd app
npm run binaries:update
```

The update script checks installed versions, downloads or builds supported tools for the current host platform, and runs smoke tests before replacing sidecar binaries.

## Notes

- RuruGrab is currently in active beta development.
- Windows and macOS release assets may appear at different times for the same version.
- Some tools are optional and may require manual setup on unsupported platforms.

## Feedback

Bug reports and feature requests are welcome in [Issues](../../issues).

## Download

Get the latest build from the [Releases](../../releases/latest) page.
