# Baryo Music

Baryo Music is a local-first Android music player for the songs already stored on your device, with a library, playback, playlist and audio tools.

**Website:** [Baryo Music](https://baryopro.github.io/BaryoMusic/) · [English page](https://baryopro.github.io/BaryoMusic/en/)

## Version 1.0.6

- **Crossfade:** optional track overlap, disabled by default.
- **Automatic online lyrics:** optional LRCLIB lookups, disabled by default; local lyrics take priority.
- **Bass Boost and equalizer:** advanced playback controls in Settings, subject to device support.
- **Library browsing:** fewer unnecessary library updates during playback progress changes.
- **Playback fix:** resolves a PCM buffer aliasing case that could interrupt Mono playback.

## APK downloads

Download the five signed install choices from the [v1.0.6 release](https://github.com/BARYOPRO/BaryoMusic/releases/tag/v1.0.6):

- `arm64-v8a` — recommended for most newer Android phones
- `armeabi-v7a` — older 32-bit ARM devices
- `x86_64` — 64-bit x86 devices and emulators
- `x86` — 32-bit x86 devices and emulators
- Universal — includes all four listed ABIs

These direct-install APKs are signed with the same Android Debug certificate as v1.0.5 so existing installations can update in place. This is not a Google Play production signing key. Keep the previous app installed when upgrading.

## Privacy

The local music library and playback history stay on the device. Automatic online lyrics are opt-in and off by default. When enabled, Baryo Music queries LRCLIB using a track's title and artist, plus album and duration when available. It does not upload audio, local lyric files, file paths or content URIs, and local lyrics are preferred.

## About this repository

This public repository contains the bilingual landing page, website styling, artwork and preview images, plus GitHub release assets for installing the app. It does **not** contain Android Kotlin/Gradle source files, app build credentials or the private source archive.

## Contact

- Email: [Ehsanfarzian2025@outlook.com](mailto:Ehsanfarzian2025@outlook.com)
- Telegram: [@OwlHapp](https://t.me/OwlHapp)
