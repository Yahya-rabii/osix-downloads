# Osix — apps that work with no internet

[Osix](https://devtools.osixlab.com) is 200+ developer tools and everyday utilities. The apps
carry all of them inside, so they open and work with **no internet connection and no browser**.
You can also download offline books (all of Wikipedia, WikiMed, repair guides) and run a small AI
assistant on your own device.

## Download

| Device | Download | Size |
|---|---|---|
| **Android** 6+ | [Osix-android.apk](https://github.com/Yahya-rabii/osix-downloads/releases/latest/download/Osix-android.apk) | ~175 MB |
| **Windows** 10/11 | [Installer](https://github.com/Yahya-rabii/osix-downloads/releases/latest/download/Osix-windows-setup.exe) · [Portable, no install](https://github.com/Yahya-rabii/osix-downloads/releases/latest/download/Osix-windows-portable.exe) | ~250 MB |
| **macOS** | [Apple silicon (M1 and newer)](https://github.com/Yahya-rabii/osix-downloads/releases/latest/download/Osix-mac-arm64.dmg) · [Intel](https://github.com/Yahya-rabii/osix-downloads/releases/latest/download/Osix-mac-x64.dmg) | ~300 MB |
| **Linux** | [Osix-linux-x86_64.AppImage](https://github.com/Yahya-rabii/osix-downloads/releases/latest/download/Osix-linux-x86_64.AppImage) | ~300 MB |

These links always give the newest version. Past versions, release notes and SHA-256 checksums
are on the [releases page](https://github.com/Yahya-rabii/osix-downloads/releases).

There is no iPhone or iPad app: Apple only allows apps from the App Store. On an iPhone, open
devtools.osixlab.com in Safari, choose **Share → Add to Home Screen**, then open Osix from that
icon once while online. It saves itself, and the icon then works offline.

## Installing

The apps are not code-signed yet, so each system asks once before the first run.

- **Android:** open the downloaded file and allow installing from this source when asked. To give
  Osix to another phone with no internet, open its Offline page and choose **Share the app**
  (Quick Share, Bluetooth, Files).
- **Windows:** run the installer, or the portable file with no install. If SmartScreen warns,
  choose **More info → Run anyway**.
- **macOS:** open the `.dmg` and drag Osix to Applications. The first time, right-click the app and
  choose **Open**.
- **Linux:** make the file executable (`chmod +x Osix-linux-x86_64.AppImage`, or Properties →
  Allow executing), then run it. No install and no root needed.

## What needs a connection

Almost nothing. The exceptions are tools whose job *is* the network: Secure Chat, online UNO and
chess, the webhook inbox, the speed test, and lookups such as DNS, SSL or WHOIS. File conversion,
image and video tools, OCR, background removal and translation run on your device when the Osix
server cannot be reached.

## About this repository

It holds only the app downloads. Osix's own source code is not public. The open-source components
inside the apps, their licences, and where to get their source are listed in [NOTICE.md](NOTICE.md).
