# PickSnap Releases

Official public release distribution channel for [PickSnap](https://picksnap.eascivo.com/) by Eascivo Studio.

PickSnap is a local photo culling workspace for macOS and Windows.

## Downloads

Current release: [v1.3.4 — release notes, checksums and build information](https://github.com/eascivo/picksnap-releases/releases/tag/v1.3.4).

| Platform | Architecture | Package |
| :--- | :--- | :--- |
| macOS | Apple Silicon (arm64) | [DMG](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.4/PickSnap-v1.3.4.dmg) |
| Windows | x64 | [Setup EXE](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.4/PickSnap-v1.3.4-Setup.exe) |
| Windows | x64 | [Portable EXE](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.4/PickSnap-v1.3.4-windows-x64.exe) · [ZIP](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.4/PickSnap-v1.3.4-windows-x64.zip) |

The macOS package is ad-hoc signed and not notarized; Windows packages are unsigned. Windows x64 binaries were built and tested under x64 emulation in a Windows 11 ARM64 UTM VM. Intel macOS and physical Windows x64 were not tested.

## What changed in 1.3.4

Card actions and star ratings stay visible, Selection Summary sits beside Export, and analysis progress with Cancel moves into the bottom status bar. Per-photo score explanations show the available technical components; scoring weights are unchanged.

Task changes save incrementally in SQLite. Upgrading preserves existing 1.3.2 tasks, backs up legacy records before migration and recovers conflicting legacy edits as separate tasks. Starting a new calculation clears previous AI results; cancellation retains the current run's completed results and manual decisions, ratings, rotations and crops.

The refreshed About window includes update status. Version 1.3.4 checks for updates at startup or manually, lets you skip a version, and can install a verified future update and restart. **Users of 1.3.2 should download and install 1.3.4 manually.**

Version 1.3.3 was withdrawn after a startup issue involving changed legacy task records. Preserve your task-data backups and contact support@eascivo.com if recovery help is needed.

Photo processing stays local. Optional CPU models require an initial download. XMP export remains off by default and can be enabled explicitly.

## Checksums and third-party sources

Verify downloads with `SHA256SUMS.txt` in the release assets. RAW decoder, GCC runtime and Windows OpenBLAS source archives are unchanged from 1.3.2 and retain their original filenames. Licenses and runtime notices are bundled with the application. See the release notes and build manifest for exact validation scope and known limitations.

## Official Links

- Official Website: [picksnap.eascivo.com](https://picksnap.eascivo.com/)
- Support & Feedback: support@eascivo.com
- Organization: [Eascivo Studio](https://github.com/eascivo)

---
© 2026 Eascivo. All rights reserved.
