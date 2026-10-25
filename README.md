# PickSnap Releases

Official public release distribution channel for [PickSnap](https://picksnap.eascivo.com/) by Eascivo Studio.

PickSnap is a local photo culling workspace for macOS and Windows.

## Downloads

Current release: [v1.3.6 — release notes, checksums and build information](https://github.com/eascivo/picksnap-releases/releases/tag/v1.3.6).

| Platform | Architecture | Package |
| :--- | :--- | :--- |
| macOS | Apple Silicon (arm64) | [DMG](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.6/PickSnap-v1.3.6.dmg) |
| Windows | x64 | [Setup EXE](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.6/PickSnap-v1.3.6-Setup.exe) |
| Windows | x64 | [Portable EXE](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.6/PickSnap-v1.3.6-windows-x64.exe) · [ZIP](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.6/PickSnap-v1.3.6-windows-x64.zip) |

The macOS package is ad-hoc signed and not notarized; Windows packages are unsigned. Windows x64 binaries were built and tested under x64 emulation in a Windows 11 ARM64 UTM VM. Intel macOS and physical Windows x64 were not tested.

## What changed in 1.3.6

PickSnap 1.3.6 improves local recommendations. On Mac, reliable Apple Vision eye observations can recover eye hints when the face detector misses a face. Independent focus and exposure scores remain unchanged.

Closely matched usable photos can receive a main-pick suggestion. Photos with strong aesthetic signals and softer detail remain available as alternatives for manual review. Severe defects, uncertain eyes and manual decisions retain their existing safeguards. Windows built-in technical references are not treated as aesthetic models. New reasons are available in all four languages.

The 1.3.5 model-download fix remains included. Models are optional and photos stay local. Users of 1.3.2 should install manually. XMP export remains off by default.

## Checksums and third-party sources

Verify downloads with `SHA256SUMS.txt` in the release assets. RAW decoder, GCC runtime and Windows OpenBLAS source archives are unchanged from 1.3.2 and retain their original filenames. Licenses and runtime notices are bundled with the application. See the release notes and build manifest for exact validation scope and known limitations.

## Official Links

- Official Website: [picksnap.eascivo.com](https://picksnap.eascivo.com/)
- Support & Feedback: support@eascivo.com
- Organization: [Eascivo Studio](https://github.com/eascivo)

---
© 2026 Eascivo. All rights reserved.
