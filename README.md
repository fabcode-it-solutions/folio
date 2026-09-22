# Folio — Read-It-Later & Article Reader App

**Folio** is a cross-platform (iOS, Android, Web) "read-it-later" application built with **Expo / React Native**. It lets users save articles from anywhere on the web and read them later in a clean, distraction-free, fully offline-capable reader — similar in spirit to Pocket or Instapaper, built from the ground up with a modern React Native stack.

This project was developed by **[The Fabcode](https://thefabcode.com)** and is shared here to showcase our engineering approach to production-grade mobile app development: offline-first architecture, real-time sync, polished UI/UX, and cross-platform delivery from a single codebase.

> This repository is shared for portfolio and reference purposes. See [LICENSE](./LICENSE) for usage terms.

---

## 🚀 What It Does

- **Save & organize articles** from any source, with tagging, favorites, and search
- **Distraction-free reader** with clean typography, light/dark themes, and reading progress
- **Works fully offline** — articles are stored locally and sync automatically once back online
- **Share extension** for iOS and Android to save articles directly from other apps in one tap
- **Import from Pocket** for users migrating from other read-it-later services
- **Real-time sync across devices** via WebSockets, so your library stays up to date everywhere
- **Multi-language support** (English, German, Spanish, French, Chinese)
- **Light, dark, and system theme modes** with a fully custom design system

---

## 📱 Platforms

| Platform | Status |
|----------|--------|
| iOS      | ✅ Native app with share extension |
| Android  | ✅ Native app with share extension |
| Web      | ✅ Full-featured PWA-style web app |

Built from a single Expo/React Native codebase — one team, one codebase, three platforms.

---

## 🛠 Tech Stack

**Frontend**
- [Expo](https://expo.dev) & React Native (SDK 53)
- [Expo Router](https://docs.expo.dev/router/introduction/) — file-based navigation
- TypeScript (strict mode) throughout

**Data & State**
- [WatermelonDB](https://watermelondb.dev/) — high-performance local-first database with bidirectional sync
- [Zustand](https://github.com/pmndrs/zustand) — lightweight, persisted app state (auth, theme)
- MMKV — fast, encrypted local storage

**UX / Design**
- Fully custom theming system (light/dark, tokens for color, type, spacing, elevation)
- Reusable themed component library (buttons, inputs, cards, tags, menus, etc.)
- i18next for internationalization

**Platform Integrations**
- Native share extensions (iOS & Android) for one-tap article saving
- WebSocket-based real-time sync engine
- EAS (Expo Application Services) for builds, OTA updates, and app store deployment

---

## 🏗 Engineering Highlights

- **Offline-first architecture** — the app is fully usable without a connection; all changes sync automatically and conflict-free once connectivity returns
- **Debounced, queued sync engine** — batches local changes and merges server updates without blocking the UI
- **Design-system-driven UI** — every screen is built from a shared set of themed primitives, keeping the app visually consistent and easy to extend
- **Type-safe end to end** — TypeScript strict mode across the app, database models, and API layer
- **Automated quality gates** — linting, formatting, and type-checking are enforced as part of the development workflow
- **CI/CD-ready** — automated build and release pipeline via EAS for iOS, Android, and Web

---

## 📂 Project Structure (High Level)

```
app/            File-based routes (screens, tabs, auth flow, article reader)
components/     Reusable UI components & themed primitives
database/       Local database models, sync engine, migrations
features/       Feature-specific logic and hooks
theme/          Design tokens, theme provider, and theming hooks
stores/         App-level state (auth, theme, persistence)
i18n/           Localization files
```

---

## 🙋 About This Project

This repository is a demonstration of the kind of production-ready, cross-platform mobile applications **The Fabcode** builds for clients — from offline-first architecture and real-time sync to polished, accessible UI.

If you're looking for a team to build or scale your mobile app, feel free to reach out via Upwork or [thefabcode.com](https://thefabcode.com).

---

© 2026 The Fabcode. All rights reserved. See [LICENSE](./LICENSE) for terms of use.
