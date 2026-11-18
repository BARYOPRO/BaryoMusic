# Baryo Music 1.5.3 — Stability Hotfix

This release focuses on freezes, ANRs and memory pressure reported on some Android devices.

## Reliability improvements

- Large playback queues are prepared off the UI thread and safely bounded.
- The visible queue uses a bounded window to avoid repeated large allocations.
- MediaStore refresh orchestration runs away from the UI dispatcher.
- Smart Performance Auto mode checks memory pressure and Android Battery Saver while playing.
- Crossfade failures are isolated so a device-specific decoder or audio-effect problem is not retried continuously.
- Artwork extraction is size-limited, concurrency-limited and written atomically.
- Lyrics reads are bounded and duplicate playlist additions are safe.

## Install options

The release provides six APK assets: `arm64-v8a`, `armeabi-v7a`, `x86_64`, `x86`, `riscv64`, and Universal. The visible app version is `1.5.3` (`versionCode` 37). These are direct-install APKs signed with the official Baryo Music certificate used for in-place updates; they are not Google Play production builds.

The public repository contains website files and APK release assets only. Android application source files, keystores and private build files are not published.
