# Roblox Space

**Made entirely by ChatGPT.** The application's interface, code, and original app icon were created by ChatGPT. Roblox, Duo, and Moonlight are independent third-party components.

Private preparation repository for the Roblox Space Windows installer, installation guide, and software update files.

**Work is still in progress. This repository is private, and the installer is being prepared as an unpublished release draft.**

## Files

| File | Purpose |
| --- | --- |
| `RobloxSpace-Setup.exe` | Standalone Windows installer. Includes the application and portable Moonlight runtime. |
| `RobloxSpace-Setup.exe.update.json` | Matching manifest for importing this installer through the application's software update window. |
| `latest.json` | Update feed manifest, prepared for a future release. |
| `Installation-Guide.html` | Step-by-step English installation and operating instructions. Download it and open it in a browser. |

Read the [installation guide](Installation-Guide.html) before configuring a new Windows installation. Repository file previews show HTML source; download the HTML file to read the formatted guide offline.

## Installation

1. Keep the computer connected to external power.
2. Close any running Roblox Space instance with its X button and wait for its game and components to exit.
3. Run `RobloxSpace-Setup.exe` and follow the installer.
4. For an existing installation, keep the original install directory. Existing pairing and phone notification settings are retained.
5. On a new Windows installation, complete First Setup, install Duo from its official release page, create the dedicated workspace, pair Moonlight, and install Roblox inside that workspace. Follow the guide in order.
6. Start the application from the desktop **Roblox Space** shortcut.

Default install directory: `%LOCALAPPDATA%\Programs\RobloxSpace`.

## Interface language

Use the top-right language selector to choose Chinese or English. The interface changes immediately without restarting the workspace, and the app remembers the selection for this Windows user. First Setup and the installer also provide a language selector. App controls, status messages, notification settings, update dialogs, and app-generated alerts follow the selected language. Roblox, Windows, and third-party components use their own language settings.

## Current behavior

- F6 starts or stops clicking once per second, after confirming a position in the screenshot picker.
- Each application launch requires a new position confirmation.
- Minimizing keeps the workspace running. X closes the game and its supporting components.
- Switching to battery power completely exits the application and workspace. Reconnecting external power does not restart them.
- Telegram and Healthchecks notifications are configured separately from software update reminders.

## Software updates

The application supports manual checks, automatic checks and reminders, verified downloads, and local installer imports. Product version metadata has not been changed.

**The private draft is not an anonymous update source. Do not enter a private release URL into the application or put a GitHub access token in an update URL.** A public, directly readable HTTPS update manifest will be configured only when publication is approved.

For a local update, keep the EXE and its matching `.update.json` file together. Import them in the software update window. The application checks file size, SHA256, and installer product information. Installation requires confirmation and a complete workspace exit. An installer containing the same application build is reported as requiring no update; run the EXE directly if a repair installation is needed.

## Scope and requirements

Windows 11 64-bit, 24H2 or later. The installer includes the portable Moonlight runtime; Duo and Roblox require separate setup. This configuration uses 1280 x 720 at 30 Hz.

This repository contains distribution files and documentation. The complete project source backup remains local and has not been uploaded. Personal passwords, bot tokens, API keys, logs, pairing profiles, and certificates are excluded.

Third-party components are provided under their respective licenses. This project is independent of Roblox Corporation.
