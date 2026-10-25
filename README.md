# PickSnap Releases

Official public release distribution channel for [PickSnap](https://picksnap.eascivo.com/) by Eascivo Studio.

PickSnap is a local photo culling workspace for macOS and Windows.

## Downloads

Current release: [v1.3.5 — release notes, checksums and build information](https://github.com/eascivo/picksnap-releases/releases/tag/v1.3.5).

| Platform | Architecture | Package |
| :--- | :--- | :--- |
| macOS | Apple Silicon (arm64) | [DMG](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.5/PickSnap-v1.3.5.dmg) |
| Windows | x64 | [Setup EXE](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.5/PickSnap-v1.3.5-Setup.exe) |
| Windows | x64 | [Portable EXE](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.5/PickSnap-v1.3.5-windows-x64.exe) · [ZIP](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.5/PickSnap-v1.3.5-windows-x64.zip) |

The macOS package is ad-hoc signed and not notarized; Windows packages are unsigned. Windows x64 binaries were built and tested under x64 emulation in a Windows 11 ARM64 UTM VM. Intel macOS and physical Windows x64 were not tested.

## What changed in 1.3.5

The optional CLIP vision model downloads from GitHub first, with the original pinned Hugging Face URL as a fallback. Both hosts use the same fixed size and SHA-256 checks. Existing valid model installations are reused.

This version fixes model download availability; recommendation algorithms and scoring are unchanged. Upgrade and retry the CLIP card in recommendation settings. Models remain optional and photos stay local.

PickSnap 1.3.4's task persistence, score explanations and built-in updater remain available. Users of 1.3.2 should install 1.3.5 manually. XMP export remains off by default.

## Checksums and third-party sources

Verify downloads with `SHA256SUMS.txt` in the release assets. RAW decoder, GCC runtime and Windows OpenBLAS source archives are unchanged from 1.3.2 and retain their original filenames. Licenses and runtime notices are bundled with the application. See the release notes and build manifest for exact validation scope and known limitations.

## Official Links

- Official Website: [picksnap.eascivo.com](https://picksnap.eascivo.com/)
- Support & Feedback: support@eascivo.com
- Organization: [Eascivo Studio](https://github.com/eascivo)

---
© 2026 Eascivo. All rights reserved.
