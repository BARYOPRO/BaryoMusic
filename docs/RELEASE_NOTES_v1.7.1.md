# Baryo Music 1.7.1 — Reliability & Security Hardening

This release hardens playback lifecycle handling, float PCM safety, MediaStore compatibility, Room-facing write concurrency, playlist duplicate handling and in-app updater memory/security behavior.

The updater now uses bounded metadata/download reads, streaming SHA-256 verification, mandatory release digests and GitHub-host allowlisting. Playback resumption respects the history privacy setting. Six signed APKs are available for arm64-v8a, armeabi-v7a, x86_64, x86, riscv64 and Universal.

No Android source code or keystores are published.
