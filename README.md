# PickSnap Releases

Official public release distribution channel for [PickSnap](https://picksnap.eascivo.com/) by Eascivo Studio.

PickSnap is a local photo culling workspace for macOS and Windows.

## Downloads

Current release: [v1.3.2 — release notes, checksums and build information](https://github.com/eascivo/picksnap-releases/releases/tag/v1.3.2).

| Platform | Architecture | Package |
| :--- | :--- | :--- |
| macOS | Apple Silicon (arm64) | [DMG](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.2/PickSnap-v1.3.2.dmg) |
| Windows | x64 | [Setup EXE](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.2/PickSnap-v1.3.2-Setup.exe) |
| Windows | x64 | [Portable EXE](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.2/PickSnap-v1.3.2-windows-x64.exe) · [ZIP](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.2/PickSnap-v1.3.2-windows-x64.zip) |

The macOS package is ad-hoc signed and not notarized; Windows packages are unsigned. Windows x64 binaries were built and tested under x64 emulation in a Windows 11 ARM64 UTM VM. Intel macOS and physical Windows x64 were not tested.

PickSnap 1.3.3 has been withdrawn following a startup issue with changed legacy task records after migration. If you used 1.3.3, preserve your task data and contact support@eascivo.com if recovery is needed. We are preparing 1.3.4.

## What changed in 1.3.2

Local portrait assistance now supports optional OCEC, NIMA and CLIP + LAION models with per-model download status. Recommendations appear in completed batches, preserve manual decisions, and support cancellation and retry. XMP export is off by default and can be enabled explicitly. Enhanced models require an initial download; photo processing stays local.

Licenses and corresponding RAW decoder sources accompany this release. See the release notes and build manifest for exact validation scope and known limitations.

## Official Links

- Official Website: [picksnap.eascivo.com](https://picksnap.eascivo.com/)
- Support & Feedback: support@eascivo.com
- Organization: [Eascivo Studio](https://github.com/eascivo)

---
© 2026 Eascivo. All rights reserved.
