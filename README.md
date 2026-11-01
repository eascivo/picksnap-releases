# PickSnap Releases

Official public release distribution channel for [PickSnap](https://picksnap.eascivo.com/) by Eascivo Studio.

PickSnap is a local photo culling workspace for macOS and Windows.

## Downloads

Current release: [v1.3.7 — release notes, checksums and build information](https://github.com/eascivo/picksnap-releases/releases/tag/v1.3.7).

| Platform | Architecture | Package |
| :--- | :--- | :--- |
| macOS | Apple Silicon (arm64) | [DMG](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.7/PickSnap-v1.3.7.dmg) |
| Windows | x64 | [Setup EXE](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.7/PickSnap-v1.3.7-Setup.exe) |
| Windows | x64 | [Portable EXE](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.7/PickSnap-v1.3.7-windows-x64.exe) · [ZIP](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.7/PickSnap-v1.3.7-windows-x64.zip) |

The macOS package is ad-hoc signed and not notarized; Windows packages are unsigned. Windows x64 binaries were built and tested under x64 emulation in a Windows 11 ARM64 UTM VM. Intel macOS and physical Windows x64 were not tested.

## What changed in 1.3.7

PickSnap 1.3.7 makes optional enhanced-model downloads more reliable. Interrupted downloads retain verified partial data and resume across retries or app restarts. Slow transfers continue while bytes arrive, while stalled reads time out and move to a backup source.

The app infers source ordering from the operating system region, including faster mainland-China sources where appropriate, and switches mirrors silently. Network-unavailable, timeout, stalled-transfer and checksum failures have clearer messages. All downloaded model files retain fixed size and SHA-256 verification before activation.

The local recommendation improvements from 1.3.6 remain included. Models are optional, photos and processing stay local, existing tasks are retained, and XMP export remains off by default.

## Checksums and third-party sources

Verify downloads with `SHA256SUMS.txt` in the release assets. RAW decoder, GCC runtime and Windows OpenBLAS source archives are unchanged from 1.3.2 and retain their original filenames. Licenses and runtime notices are bundled with the application. See the release notes and build manifest for exact validation scope and known limitations.

## Official Links

- Official Website: [picksnap.eascivo.com](https://picksnap.eascivo.com/)
- Support & Feedback: support@eascivo.com
- Organization: [Eascivo Studio](https://github.com/eascivo)

---
© 2026 Eascivo. All rights reserved.
