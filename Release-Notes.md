# Roblox Space

English | [Chinese / 华语](Release-Notes.zh-Hans.md)

**[Download the Windows installer](https://github.com/jasonhome-344423/roblox-space/releases/latest/download/RobloxSpace-Setup.exe)**

[Download the installation guide — Chinese / English](https://github.com/jasonhome-344423/roblox-space/releases/latest/download/Installation-Guide.html)

## Included

- One official application with an EXE installer and portable Moonlight runtime.
- Chinese and English interfaces, immediate language switching, and a complete offline installation guide.
- Screenshot position confirmation and F6 control for clicking once per second inside the configured workspace.
- Roblox disconnect monitoring, reconnect controls, Telegram phone messages, and Healthchecks network-outage alerts.
- Background phone-notification verification and timeout retries.
- More reliable viewer startup handling and additional diagnostic-log fallback paths.
- Recoverable saving of language and phone-alert preferences in encrypted user folders.

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

## Installation and integrity

The in-application software updater has been removed, including update checks, reminders, installer downloads, and local-installer import. If you choose to install the application again, download the EXE from this release and run it manually after closing Roblox Space.

**SHA256SUMS.txt** lists release-file hashes. The complete project-source backup remains local; this release excludes personal settings and credentials.

**Made entirely by ChatGPT:** the application's interface, code, and original icon. Roblox, Duo, and Moonlight are independent third-party components with their own authorship and licenses.

## Language coverage

The main and monitor windows, click and position controls, notification settings, messages sent by this application, errors, dialog buttons, First Setup, installer, folder picker, and uninstaller support Chinese and English. Recovery commands include both languages and provide English and Chinese filenames. The offline guides contain matching detailed installation, notification, recovery, and troubleshooting steps.

Third-party Windows prompts, games, Duo, Moonlight, Telegram, and Healthchecks pages and automatic messages use their own language settings. Technical identifiers, user input, and original system diagnostics retain their original text.

## Distribution and troubleshooting details

The installer is currently **unsigned**. Download it from this repository's release, compare its SHA256 against `SHA256SUMS.txt` from the same release, and read the SmartScreen instructions at the start of the bilingual guide. A matching hash does not replace publisher signing; do not disable Windows protection.

Original Moonlight, Qt, and runtime license/copyright texts, pinned source locations, material checksums, and unmodified Moonlight source/build recipes are included in `runtime/Moonlight/licenses` and `NOTICE.txt`. The release also provides **Third-Party-Notices.zip** for inspection without running the installer. Complete Qt sources are linked by their fixed version in the notice; they are not all embedded in the small offline recovery package.

Use a **dedicated Healthchecks project containing only this application's check** and that project's read-write API key. The key has project-wide permissions. The guide explains transferring an existing check, retaining its Ping URL, and setting up the new project's Telegram integration and key. This installer does not move existing cloud configuration automatically.

There is no product version label. Tray **About** and the first log entry of each session show the build hash and UTC build time. `manifest.json` is the source backup's file inventory. ZIP entry and manifest paths use `/`. The backup keeps one complete bilingual guide at its root plus editable language templates; the Chinese HTML filename is a lightweight entry point.