# Title Bar Theme for Chrome Remote Desktop

A lightweight, zero-configuration Chrome extension that matches the window title bar and startup screen of the **Chrome Remote Desktop** desktop app in Chrome to your active Light or Dark theme.

## What Is This Project?

When you install and run [Chrome Remote Desktop](https://remotedesktop.google.com/) as a standalone Chrome app on Windows, it opens in its own dedicated window with a native desktop title bar across the top. This extension automatically keeps that window title bar and the app's startup screen synchronized with your active Light or Dark theme.

## Why Does It Exist?

By default, Chrome Remote Desktop does not provide a title bar color to Chrome at all, leaving the installed app window with an unthemed default title bar that clashes with Dark mode, Light mode, and dimmed pop-up dialogs (such as PIN entry, host setup, or settings).

This extension solves that automatically with zero settings to manage:

- Switches the window title bar seamlessly between Light and Dark modes to match the Chrome Remote Desktop interface.
- Dims smoothly in real time whenever a pop-up dialog opens and restores cleanly when dismissed.
- Remembers your active theme locally so launching the app opens with a matching startup screen instead of flashing an unthemed title bar.

> [!NOTE]
> Window title bar coloring applies to **standalone Chrome app windows** (created via Chrome's **menu (`⋮`) → Cast, save, and share → Install page as app…**). Regular Chrome browser tabs use Chrome's normal tab strip and are unaffected.

## Installation

### Option 1: Chrome Web Store (Recommended)

1. Open the extension listing on the Chrome Web Store: [Title Bar Theme for Chrome Remote Desktop](https://chromewebstore.google.com/detail/goeedkphpabkkmajcmngohomgmdodgaf).
2. Click **Add to Chrome**.
3. Open the Chrome Remote Desktop app—your title bar updates automatically with no further setup.

### Option 2: Chrome Developer Mode (Local Setup)

1. Clone or download this repository to a folder on your computer.
2. Open Google Chrome and go to `chrome://extensions/`.
3. Turn on **Developer mode** using the toggle in the top-right corner.
4. Click **Load unpacked** in the top-left and select the root folder of this repository (the folder containing `manifest.json`).
5. Open **Chrome Remote Desktop** (`https://remotedesktop.google.com/access/`) in its standalone Chrome app window.

## Documentation

- [**Technical Documentation**](./docs/technical.md) — Architecture, implementation details, and design rationale.
- [**Privacy Policy**](./docs/privacy.md) — Privacy details (zero data collection; all theme detection runs locally in your browser).
