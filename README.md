# RuruGrab

[![Latest release](https://img.shields.io/github/v/release/RuruBros/RuruGrab-Releases?display_name=tag&sort=semver)](https://github.com/RuruBros/RuruGrab-Releases/releases/latest)
[![Total downloads](https://img.shields.io/github/downloads/RuruBros/RuruGrab-Releases/total)](https://github.com/RuruBros/RuruGrab-Releases/releases)
![Platforms](https://img.shields.io/badge/platform-Windows%20x64%20%7C%20macOS%20Apple%20Silicon-2563eb)
![Status](https://img.shields.io/badge/status-beta-f59e0b)

**README:** [English](README.md) · [한국어](README.ko-KR.md) · [日本語](README.ja.md) · [简体中文](README.zh-CN.md)

RuruGrab is a local-first desktop workspace for downloading web media, capturing text, organizing files, and keeping everyday utilities in one app.

> RuruGrab is in active beta. Back up important data and review the release notes before updating.

## Download

### [Download the latest release](https://github.com/RuruBros/RuruGrab-Releases/releases/latest)

Choose the manual installer for your platform:

| Platform | Download this asset | Architecture |
| --- | --- | --- |
| macOS | `RuruGrab_<version>_aarch64.dmg` | Apple Silicon (M1 or newer) |
| Windows | `RuruGrab_<version>_x64-setup.exe` | x86-64 |

Not every release necessarily contains both platform builds. If the installer for
your platform is not attached to the latest release, check the other releases for
the newest compatible build.

The following files are primarily for RuruGrab's built-in updater and are not the normal manual installers:

- `latest.json`
- `*.app.tar.gz`
- `*.nsis.zip`

A macOS `*.app.zip` file is also provided as an alternative manual package. For the simplest installation, use the `.dmg`.

Release downloads are relatively large because RuruGrab bundles the media tools and browser runtime required by supported workflows.

## Installation

### macOS

1. Download the `aarch64.dmg` asset from the latest compatible release.
2. Open the disk image.
3. Drag `RuruGrab.app` to the `Applications` folder.
4. Launch RuruGrab from `Applications`.

Public macOS builds are signed and notarized. If macOS still blocks the first
launch, open **System Settings → Privacy & Security** and review the message shown
for RuruGrab before choosing **Open Anyway**.

### Windows

1. Download the `x64-setup.exe` asset from the latest compatible release.
2. Run the installer.
3. Launch RuruGrab from the Start menu or its installed location.

## Highlights

### Grab web content

- Queue and manage media downloads from supported websites.
- Use the Chrome or Edge companion extension to send supported pages to the desktop app.
- Extract web text into Markdown and search saved content later.
- Search and organize media metadata when the feature is available for your account.

### Organize files and media

- Organize files with reusable rules.
- Batch rename files with a preview before applying changes.
- Find duplicate files using configurable comparisons.
- Create GIFs from local media and generate QR codes.

### Keep a local workspace

- Build searchable OneSpace catalogs for files spread across folders and drives.
- Write in Notepad and Mind Map tools.
- Store private notes in an encrypted Vault protected by a master password.
- Use remote file, chat, automation, integration, and diagnostic tools as needed.

Feature availability can vary by platform, account access, and local configuration.

## Browser Companion

The browser extension is bundled with the desktop app and currently uses Chrome or Edge developer mode.

1. Open `chrome://extensions/` or `edge://extensions/`.
2. Enable **Developer mode**.
3. Select **Load unpacked**.
4. Select RuruGrab's bundled `extension` directory.

Typical locations:

```text
Windows: C:\Users\<YourUserName>\AppData\Local\RuruGrab\extension
macOS:   /Applications/RuruGrab.app/Contents/Resources/extension
```

On macOS, right-click `RuruGrab.app`, choose **Show Package Contents**, and open `Contents/Resources/extension`.

Keep the desktop app running when using extension actions that send data to RuruGrab. The extension communicates with the app through a local API on `127.0.0.1`.

## Updates

RuruGrab checks its platform-specific GitHub release channel after launch. You can
also click the version number in the app sidebar to check manually, download an
available update, and restart into the new version.

## Local-first by default

Core app data is stored on your device by default. Network access is used only by
features that require it, such as user-requested downloads, metadata lookup,
update checks, remote connections, and integrations that you configure.

## Languages

The app UI currently includes:

- English
- 한국어
- 日本語
- 简体中文
- 繁體中文
- Español
- Français
- Deutsch
- Português (Brasil)
- Русский

## Feedback

Please use [GitHub Issues](https://github.com/RuruBros/RuruGrab-Releases/issues) for bug reports and feature requests.

When reporting a problem, include the RuruGrab version, operating system, steps to
reproduce, and relevant diagnostics. Remove passwords, tokens, cookies, personal
file paths, and other sensitive data before posting logs or screenshots.
