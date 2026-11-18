# Baryo Music

Baryo Music is a local-first Android music player for the songs already stored on your device, with library, playback, playlist, audio clarity and Smart Performance tools.

**Website:** [Baryo Music](https://baryopro.github.io/BaryoMusic/) · [English page](https://baryopro.github.io/BaryoMusic/en/)

## Latest stable release: 1.6.9

This stability hotfix focuses on freezes, ANRs and memory pressure reported on some Android devices.

- Large playback queues are prepared off the UI thread and safely bounded.
- The visible queue uses a bounded window so very large libraries do not trigger repeated allocations.
- MediaStore refresh orchestration is kept off the UI dispatcher.
- Smart Performance Auto mode checks memory pressure and Android Battery Saver while playing.
- Crossfade failures are isolated so a device-specific decoder or audio-effect problem is not retried continuously.
- Artwork extraction is size-limited, concurrency-limited and written atomically.
- Lyrics reads are bounded and duplicate playlist additions are safe.
- The Home carousel includes Smart Performance and ClearSound as polished fifth and sixth slides.
- ClearSound provides Natural, Balanced and Night modes with K-weighted short-term stable peak protection normalization, an adjustable -18 to -8 stable peak protection target, and true-peak safety.

## APK downloads

Download the six signed install choices from the [v1.6.9 Stability Hotfix release](https://github.com/BARYOPRO/BaryoMusic/releases/tag/v1.6.9):

- `arm64-v8a` — recommended for most newer Android phones
- `armeabi-v7a` — older 32-bit ARM devices
- `x86_64` — 64-bit x86 devices and emulators
- `x86` — 32-bit x86 devices and emulators
- `riscv64` — RISC-V Android devices where supported
- Universal — includes the supported ABI payloads

These direct-install APKs are signed with the same Baryo Music certificate used for previous releases so existing installations can update in place. This is not a Google Play production signing key. Keep the previous app installed when upgrading.

## Privacy

The local music library and playback history stay on the device. Automatic online lyrics are opt-in and off by default. When enabled, Baryo Music queries LRCLIB using a track's title and artist, plus album and duration when available. It does not upload audio, local lyric files, file paths or content URIs, and local lyrics are preferred.

## About this repository

This public repository contains the bilingual landing page, website styling, artwork and preview images, plus GitHub release assets for installing the app. It does **not** contain Android Kotlin/Gradle source files, app build credentials, keystores or the private source archive.

## Contact

- Email: [Ehsanfarzian2025@outlook.com](mailto:Ehsanfarzian2025@outlook.com)
- Telegram: [@OWLHAPPY](https://t.me/OWLHAPPY)


### 1.6.9 Reliability hardening

The latest hotfix hardens updater memory use, MediaStore compatibility, playback resumption privacy, PCM float safety, playlist concurrency and Favorites/History writes.
