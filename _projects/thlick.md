---
layout: page
title: Thlick
description: A native macOS menu bar app that plays mechanical keyboard sounds as you type, in any app.
img: assets/img/project/thlick.png
importance: 1
category: work
github: https://github.com/khamkarsuraj/thlick
---

### Project Overview

Thlick is a free, open-source macOS utility that lives in the menu bar and plays a mechanical keyboard sound for every key you press, system-wide. It ships with four sound profiles (Cobalt, Walnut, Onyx and Ember), mutes itself while the microphone is in use, supports per-app exclusions and global shortcuts, and runs as a signed, notarized universal binary on macOS 13 Ventura and later.

Privacy is built in: the key listener is listen-only and only sees the key category, never the characters. Nothing is stored or sent anywhere, and password fields are skipped.

---

### Links

- Website: [https://thlick.com](https://thlick.com)
- Source code: [https://github.com/khamkarsuraj/thlick](https://github.com/khamkarsuraj/thlick)
- Download: [Releases](https://github.com/khamkarsuraj/thlick/releases)

---

### Features

- **System-wide sounds**: one sound per keypress in any app, with a sub-20 ms key-to-sound latency target.
- **Four profiles**: Cobalt (sharp), Walnut (soft, office-friendly), Onyx (deep thock) and Ember (light, quiet).
- **Menu bar first**: popover controls, timed mute, optional Dock icon and launch at login.
- **Auto-mute**: goes silent while the microphone is in use, with per-app exclusions for apps that should stay quiet.
- **Global shortcuts**: toggle sound, mute, volume and profile from anywhere, with an on-screen HUD and cheat sheet.
- **Accessible**: VoiceOver, keyboard navigation, Reduce Motion, and light and dark mode.

---

### Technology Stack

- **App**: Swift and SwiftUI, sandboxed, with separate direct-download and Mac App Store targets
- **Audio**: low-latency sound engine measured with a repeatable latency bench
- **Testing and CI**: Swift Testing unit tests, GitHub Actions on Apple silicon and Intel runners
- **Distribution**: Developer ID signed and notarized DMG
