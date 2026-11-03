# Roblox Space

A Windows application that brings a configured Roblox workspace, click controls, disconnect monitoring, and phone alerts into one window.

**Made entirely by ChatGPT:** the application's interface, code, and original icon. Roblox, Duo, and Moonlight are independent third-party components with their own authorship and licenses.

## Download

### [Download Roblox Space for Windows — EXE installer](https://github.com/jasonhome-344423/roblox-space/releases/latest/download/RobloxSpace-Setup.exe)

- [Latest release and all download files](https://github.com/jasonhome-344423/roblox-space/releases/latest)
- [Installation guide — Chinese / English](https://github.com/jasonhome-344423/roblox-space/releases/latest/download/Installation-Guide.html)
- [Release-file SHA256 checksums](https://github.com/jasonhome-344423/roblox-space/releases/latest/download/SHA256SUMS.txt)

**For installation, download `RobloxSpace-Setup.exe` from the release assets and run it.** The HTML guide has Chinese / English buttons and works offline after download. GitHub's automatic source archives contain this distribution repository's files, not the complete local project-source backup.

## Install and start

1. Keep the computer connected to external power.
2. For an upgrade, close Roblox Space with X and wait for its game, monitor, and viewer to exit.
3. Run `RobloxSpace-Setup.exe`. Keep the existing installation directory when upgrading.
4. On a new Windows installation, follow the guide's Windows, Duo, account, pairing, and Roblox setup steps in order.
5. Open the desktop **Roblox Space** shortcut and approve the Windows permission prompt.
6. Enter a game, confirm a safe position with the screenshot picker, then press **F6** to toggle clicking once per second.

The default install directory is `%LOCALAPPDATA%\Programs\RobloxSpace`. Upgrades retain existing pairing and phone notification settings. An ordinary application upgrade does not require another Windows account, a new Telegram bot, or another Duo installation.

## Start, minimize, and exit

- The desktop shortcut starts the required workspace components together.
- **Minimize** keeps the game, monitoring, and clicking running.
- **X** closes the game, clicking, monitor, Moonlight viewer, and application. It retains the Duo workspace for faster reopening.
- To also stop Duo, right-click the application tray icon while Roblox Space is open and choose **Exit everything (including Duo)**.
- Switching to battery while the application is running performs a complete shutdown. Returning to external power does not reopen it.
- Once the application has exited, it no longer monitors power changes or sends cloud heartbeats. Normal exit attempts to pause the cloud check.

The first launch after a Windows restart or complete Duo shutdown needs to create the workspace again. Reusing a retained workspace is usually faster; startup time varies with the computer and system state.

## Controls and languages

F6 starts or stops clicking once per second. A fresh application launch requires another screenshot position confirmation. Stop automatic clicking before using the keyboard-input action. Click controls operate inside the configured workspace.

The application, installer, and First Setup support Chinese and English. The application's top-right selector changes its interface immediately and remembers the choice for the current Windows user. The offline guide has a separate language selector. Roblox and Windows retain their own language settings.

## Monitoring and phone alerts

Roblox disconnect monitoring waits for a confirmed connection and new disconnect evidence; opening the Roblox home screen is not the same as joining a game server.

Telegram handles direct phone messages. Healthchecks monitors missing computer heartbeats from outside the computer. Both require the setup described in the guide. The application sends cloud heartbeats about every 30 seconds; the configured cloud alert is expected about two minutes after the last received heartbeat. It does not wait for Roblox to disconnect, and exact phone delivery time is not guaranteed.

A Telegram timeout is displayed as retrying, not as an expired bot token. Verification retries run in the background. Keep the application open for monitoring and use mobile data on the phone when testing a complete computer network outage.

## Manual installation

The in-application software updater has been removed. Roblox Space does not check for software updates, display update reminders, download installers, or import installers through the application.

If you choose to reinstall or obtain another installer, download **RobloxSpace-Setup.exe** from the [release page](https://github.com/jasonhome-344423/roblox-space/releases/latest) in your browser. Close Roblox Space, run the EXE yourself, and retain the existing installation directory to keep your pairing and phone-alert settings.
## Requirements and scope

Windows 11 x64, 24H2 or later. The installer includes portable Moonlight. Duo and Roblox require the separate setup in the guide. This configuration uses **1280 × 720 at 30 Hz** with the free Duo configuration; it does not promise 60 or 120 Hz.

The internal account `RobloxSpaceBeta` and Duo instance `RobloxBeta` are retained for compatibility with the existing workspace. Do not delete them as unused test files.

This repository distributes the installer, documentation, and release-file checksums. The complete project-source backup remains local. Personal passwords, bot tokens, API keys, logs, pairing profiles, and certificates are excluded.

This project is independent of Roblox Corporation. Third-party components retain their respective licenses.