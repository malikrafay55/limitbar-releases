# Limitbar releases

Downloads for **Limitbar**, a small Windows 11 (and Linux) tray app that shows
how much of your AI subscription limits you have used (Claude, ChatGPT/Codex,
Gemini, Grok), with an optional Dynamic Island pill at the top of the screen.

This repository holds release binaries and the update manifest only. The app
checks it for updates (Settings → Updates).

## Install

Get the files from the [latest release](../../releases/latest).

- **Windows 10/11 x64**: `Limitbar_<version>_x64-setup.exe`. It's a per-user
  installer and installs WebView2 if needed. The build is not code-signed, so
  SmartScreen asks once: *More info → Run anyway*.
- **Linux (x86_64)**:
  - `.deb`: `sudo apt install ./Limitbar_<version>_amd64.deb`
  - AppImage: `chmod +x Limitbar_<version>_amd64.AppImage` and run it.
  - Needs GNOME Keyring or KWallet (credentials are kept in the system
    keyring) and a tray with AppIndicator support.

## Privacy

Limitbar talks only to the AI providers you add and to this repository for
update checks. It sends no telemetry. Credentials stay in your system keyring.
