# PickSnap Releases

Official public release distribution channel for [PickSnap](https://picksnap.eascivo.com/) by Eascivo Studio.

PickSnap is a local photo culling workspace for macOS and Windows.

## Downloads

Current release: [v1.3.8 — release notes, checksums and build information](https://github.com/eascivo/picksnap-releases/releases/tag/v1.3.8).

| Platform | Architecture | Package |
| :--- | :--- | :--- |
| macOS | Apple Silicon (arm64) | [DMG](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.8/PickSnap-v1.3.8.dmg) |
| Windows | x64 | [Setup EXE](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.8/PickSnap-v1.3.8-Setup.exe) |
| Windows | x64 | [Portable EXE](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.8/PickSnap-v1.3.8-windows-x64.exe) · [ZIP](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.8/PickSnap-v1.3.8-windows-x64.zip) |

The macOS package is ad-hoc signed and not notarized; Windows packages are unsigned. Windows x64 binaries were built and tested under x64 emulation in a Windows 11 ARM64 UTM VM. Intel macOS and physical Windows x64 were not tested.

## What changed in 1.3.8

PickSnap 1.3.8 improves the in-app update experience and adds optional anonymous usage statistics. The app can check for stable releases silently at launch and offer Update Now, Not Now, or a version-specific Skip (with a reminder control in About). Stable release metadata is cached for 12 hours, revalidated with ETags, shared with the installer, and backs off on rate limits.

Anonymous statistics use a resettable random ID, a bounded local queue, a privacy notice and opt-out. Photos, paths and personal content are never included. Optional enhanced-model download reliability from 1.3.7 and the local recommendation improvements from 1.3.6 remain included.

## Checksums and third-party sources

Verify downloads with `SHA256SUMS.txt` in the release assets. RAW decoder, GCC runtime and Windows OpenBLAS source archives are unchanged from 1.3.2 and retain their original filenames. Licenses and runtime notices are bundled with the application. See the release notes and build manifest for exact validation scope and known limitations.

## Official Links

- Official Website: [picksnap.eascivo.com](https://picksnap.eascivo.com/)
- Support & Feedback: support@eascivo.com
- Organization: [Eascivo Studio](https://github.com/eascivo)

---
© 2026 Eascivo. All rights reserved.
