# Baryo Music 1.0.6

## Highlights

- **Crossfade** adds overlapping transitions between tracks. It is optional and disabled by default.
- **Automatic online lyrics** uses LRCLIB only when the user opts in; it is disabled by default and local lyrics always take priority. When enabled, the lookup sends the track title and artist, plus album and duration when available. Audio, file paths, content URIs and local lyric files are not uploaded.
- **Bass Boost and equalizer** controls are available in Settings; effect support depends on the Android device.
- Library progress updates avoid unnecessary repeated library work while scrolling.
- Fixed a PCM buffer aliasing case that could interrupt Mono playback.

## Install options

The release provides five signed APKs: `arm64-v8a`, `armeabi-v7a`, `x86_64`, `x86`, and Universal. The visible app version is `1.0.6` (`versionCode` 14), and the signing certificate matches v1.0.5 for in-place updates. These are direct-install APKs signed with Android's Debug certificate, not a Google Play production key.

The public release contains APK assets only; Android application source files are not attached.
