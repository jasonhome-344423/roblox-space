# Roblox Space

A Windows application for the configured Roblox workspace, clicking controls, disconnect monitoring, and phone alerts.

**Made entirely by ChatGPT:** application interface, code, and original app icon. Roblox, Duo, and Moonlight are independent third-party components.

## Download

### [Download Roblox Space 1.0.0 for Windows — EXE installer](https://github.com/jasonhome-344423/roblox-space/releases/download/v1.0.0/RobloxSpace-Setup.exe)

- [Latest release and all download files](https://github.com/jasonhome-344423/roblox-space/releases/latest)
- [Download the installation guide — Chinese / English](https://github.com/jasonhome-344423/roblox-space/releases/download/v1.0.0/Installation-Guide.html)
- [Installer update manifest](https://github.com/jasonhome-344423/roblox-space/releases/download/v1.0.0/RobloxSpace-Setup.exe.update.json)
- [Release-file SHA256 checksums](https://github.com/jasonhome-344423/roblox-space/releases/download/v1.0.0/SHA256SUMS.txt)

**To install the application, download `RobloxSpace-Setup.exe` from the release assets.** Download the HTML guide and open it in a browser; its Chinese / English buttons work offline. GitHub's automatic source archives contain this distribution repository's files, not the complete local project-source backup.

## Install and start

1. Keep the computer connected to external power.
2. For an upgrade, close Roblox Space with its X button and wait for the game and supporting processes to exit.
3. Run `RobloxSpace-Setup.exe` and keep the existing installation directory when upgrading.
4. On a new Windows installation, follow the guide's Windows, Duo, account, pairing, and Roblox setup steps in order.
5. Open the desktop **Roblox Space** shortcut.

Default install directory: `%LOCALAPPDATA%\Programs\RobloxSpace`. Existing pairing and phone notification settings are retained during an upgrade.

## Languages

The application, installer, and First Setup support Chinese and English. Use the top-right selector in the application to switch immediately; the choice is remembered for this Windows user. The installation guide has its own language buttons and remembers its selection in the browser. Roblox and Windows use their own language settings.

## Features

- F6 starts or stops clicking once per second, after confirming a position with the screenshot picker. Each launch requires position confirmation.
- Disconnect monitoring and reconnect controls operate inside the configured workspace.
- Minimizing keeps the workspace running. X exits the application and closes its game and supporting processes.
- Switching to battery completely exits the application and workspace. Returning to external power does not reopen them.
- Telegram and Healthchecks phone alerts use independent background verification. Telegram timeouts are displayed as retrying; they are not described as expired bot tokens.
- Software updates support manual and automatic checks, reminders, verified downloads, and local installer import.

## Software updates

Version numbering starts at **1.0.0** and follows **major.minor.patch**: major releases change the first number, smaller feature updates the second, and fixes or patches the third. A matching Beta channel uses the same base version with a Beta label.

Official update feed:

```text
https://raw.githubusercontent.com/jasonhome-344423/roblox-space/main/latest.json
```

New installations configure this feed automatically. Existing installations can save it in **Software Updates**, enable automatic reminders, and choose **Check Updates**. Updates are installed only after confirmation and a complete workspace exit. For local import, keep the EXE and its matching `.update.json` together.

## Requirements and scope

Windows 11 x64, 24H2 or later. The installer includes portable Moonlight; Duo and Roblox require the setup described in the guide. This configuration uses 1280 × 720 at 30 Hz.

This repository distributes the installer, documentation, and update manifests. The complete project-source backup remains local. Personal passwords, bot tokens, API keys, logs, pairing profiles, and certificates are excluded.

Third-party components retain their respective licenses. This project is independent of Roblox Corporation.