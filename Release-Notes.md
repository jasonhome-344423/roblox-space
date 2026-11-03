# Roblox Space

**[Download the Windows installer](https://github.com/jasonhome-344423/roblox-space/releases/latest/download/RobloxSpace-Setup.exe)**

[Download the installation guide — Chinese / English](https://github.com/jasonhome-344423/roblox-space/releases/latest/download/Installation-Guide.html)

## Included

- One official application with an EXE installer and portable Moonlight runtime.
- Chinese and English interfaces, immediate language switching, and a complete offline installation guide.
- Screenshot position confirmation and F6 control for clicking once per second inside the configured workspace.
- Roblox disconnect monitoring, reconnect controls, Telegram phone messages, and Healthchecks network-outage alerts.
- Background notification verification, timeout retries, software update checks, reminders, and verified local or downloaded installers.
- More reliable viewer startup handling and additional diagnostic-log fallback paths.
- Recoverable saving of update, language, and phone-alert preferences in encrypted user folders.

## Startup and exit behavior

The desktop shortcut starts the workspace components together. Normal **X** closes the game, clicking, monitor, Moonlight viewer, and application while retaining the Duo workspace for faster reopening. To close Duo as well, right-click the application tray icon while Roblox Space is open and select **Exit everything (including Duo)**.

Switching to battery while the application is running exits everything. Reconnecting power does not restart it. The application no longer monitors power or network state once it has exited. Minimizing keeps it running.

The first start after a Windows restart or complete Duo shutdown requires the desktop to be created again. Startup times depend on the computer and current system state.

## Install

1. Download **RobloxSpace-Setup.exe** from the assets below and run it.
2. For an upgrade, close Roblox Space first and retain the existing installation directory. Pairing and notification settings are kept.
3. For a new Windows installation, download **Installation-Guide.html**, choose Chinese or English, and complete its setup steps in order.
4. Start **Roblox Space** from its desktop shortcut and approve the Windows permission prompt.
5. Enter a game and confirm a new click position before using F6.

Windows 11 x64, 24H2 or later is required. Duo and Roblox need the separate setup described in the guide. Portable Moonlight is included. The configured workspace uses **1280 × 720 at 30 Hz**.

## Updates and integrity

The application and release titles do not use visible product version numbers. Updates identify installation content using a build fingerprint. New installations use the official [update feed](https://raw.githubusercontent.com/jasonhome-344423/roblox-space/main/latest.json).

Keep **RobloxSpace-Setup.exe.update.json** beside the EXE when importing a local update. **SHA256SUMS.txt** lists release-file hashes. The complete project-source backup remains local; this release excludes personal settings and credentials.

**Made entirely by ChatGPT:** the application's interface, code, and original icon. Roblox, Duo, and Moonlight are independent third-party components with their own authorship and licenses.
