# RuruGrab

[![Latest release](https://img.shields.io/github/v/release/RuruBros/RuruGrab-Releases?display_name=tag&sort=semver)](https://github.com/RuruBros/RuruGrab-Releases/releases/latest)
[![Total downloads](https://img.shields.io/github/downloads/RuruBros/RuruGrab-Releases/total)](https://github.com/RuruBros/RuruGrab-Releases/releases)
![Platforms](https://img.shields.io/badge/platform-Windows%20x64%20%7C%20macOS%20Apple%20Silicon-2563eb)
![Status](https://img.shields.io/badge/status-beta-f59e0b)
![App languages](https://img.shields.io/badge/app-EN%20%7C%20KO%20%7C%20JA%20%7C%20ZH--CN%20%7C%20ES%20%7C%20PT--BR-16a34a)

**Language guides:** English · [한국어](https://rurubros.org/rurugrab/?lang=ko) · [日本語](https://rurubros.org/rurugrab/?lang=ja) · [简体中文](https://rurubros.org/rurugrab/?lang=zh-CN) · [Español](https://rurubros.org/rurugrab/?lang=es) · [Português (Brasil)](https://rurubros.org/rurugrab/?lang=pt-BR)

[Official site](https://rurubros.org/rurugrab/) · [Latest release](https://github.com/RuruBros/RuruGrab-Releases/releases/latest) · [All releases](https://github.com/RuruBros/RuruGrab-Releases/releases)

RuruGrab connects Chrome or Edge to a local-first desktop toolkit for saving web media, tracking what you watched, extracting text, and organizing the files that follow.

> RuruGrab is in active beta. Back up important data and review the release notes before updating.

## Download

### [Download the latest release](https://github.com/RuruBros/RuruGrab-Releases/releases/latest)

Choose the manual installer for your platform:

| Platform | Download this asset | Architecture |
| --- | --- | --- |
| macOS | `RuruGrab_<version>_aarch64.dmg` | Apple Silicon (M1 or newer) |
| Windows | `RuruGrab_<version>_x64-setup.exe` | x86-64 |

Not every release necessarily contains both platform builds. If the newest release has no installer for your platform, check [all releases](https://github.com/RuruBros/RuruGrab-Releases/releases) for the latest compatible build.

`latest.json`, `*.app.tar.gz`, and `*.nsis.zip` are primarily updater assets. A macOS `*.app.zip` is also available as an alternative manual package; the `.dmg` is the simplest installation choice.

Release downloads are relatively large because RuruGrab bundles the media tools and browser runtime required by supported workflows.

## What RuruGrab does

### Grab web content

- Queue supported pages from the desktop app or the Chrome/Edge companion extension.
- Download video, audio, images, galleries, torrents, and remote files.
- Extract supported page text into Markdown and browse it later.
- Monitor progress, retry or cancel tasks, and manage several selected queue rows at once.
- Search and curate provider metadata when the feature is available for your account.

### Current source connections

| Source family | Supported workflow |
| --- | --- |
| YouTube | Videos, Shorts, audio-only actions, authenticated retries, and watched markers |
| Bilibili | Video pages, including a selected multipart `p` value |
| TikTok | Video, embed, and supported share links |
| SOOP | VOD player pages and supported VOD aliases |
| iMBC, Naver TV, CHZZK, PandaLive, Facebook | Supported video or live-page routes |
| X / Twitter, Instagram, Pinterest, Pixiv | Media and gallery routes |
| RidiBooks, Munpia, generic HTML pages | Text extraction to Markdown |
| Magnet links and `.torrent` files | Preview, file selection, limits, and local download |
| WebDAV, SFTP, FTP, FTPS | Remote browsing and queued file transfer |

Availability can depend on the page type, region, account access, cookies supplied for an authenticated retry, and upstream site or extractor changes. RuruGrab does not claim that every URL on a listed domain is downloadable.

### Organize local files

- Use the unified Files workspace to organize by rules, preview batch renames, and review duplicate groups before cleanup.
- Build searchable OneSpace catalogs across folders and drives.
- Trim and style local media in GIF Maker, and create configurable QR codes.

### Work in Studio

- **PLIORA** combines connected notes, rich text, semantic zoom, search, auto-arrange, and JSON import/export on a spatial canvas.
- **CERUNE** keeps private notes encrypted locally behind a master password.

### Connect optional tools

- Browse remote locations and queue downloads from them.
- Connect an XMPP account for in-app chat.
- Configure external tools and Telegram bot profiles in Integration.
- Inspect local server status, updates, logs, database tables, and diagnostics.

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

Keep the desktop app running for extension actions that send or sync data. The extension connects through RuruGrab's token-protected local API on `127.0.0.1`; it can queue supported pages, sync or restore watched history, and show RuruGrab watched markers on supported YouTube surfaces.

## Installation

### macOS

1. Download the `aarch64.dmg` asset from the latest compatible release.
2. Open the disk image and drag `RuruGrab.app` to `Applications`.
3. Launch RuruGrab from `Applications`.

Public macOS builds are signed and notarized. If macOS still blocks the first launch, open **System Settings → Privacy & Security**, review the RuruGrab message, and choose **Open Anyway** only after confirming the download came from this repository.

### Windows

1. Download the `x64-setup.exe` asset from the latest compatible release.
2. Run the installer.
3. Launch RuruGrab from the Start menu or its installed location.

## Official site and account connection

The official product page is [rurubros.org/rurugrab](https://rurubros.org/rurugrab/). Optional account-backed features authenticate through RuruBros Central Identity on `rurubros.org`; availability still depends on the RuruGrab account's access. Core local tools and local data do not become cloud storage because an account is connected.

## Updates and local-first behavior

RuruGrab checks its platform-specific GitHub release channel after launch. You can also click the version number in the sidebar to check manually, download an update, and restart into the new version.

Core app data stays on your device by default. Network access is used for actions that require it, including requested downloads, enabled site and metadata providers, update checks, remote connections, account authentication, and integrations you configure.

## App languages

The desktop app and browser companion share six supported interface languages: English, 한국어, 日本語, 简体中文, Español, and Português (Brasil).

## Feedback

Please use [GitHub Issues](https://github.com/RuruBros/RuruGrab-Releases/issues) for bug reports and feature requests.

Include the RuruGrab version, operating system, steps to reproduce, and relevant diagnostics. Remove passwords, tokens, cookies, personal file paths, and other sensitive data before posting logs or screenshots.
