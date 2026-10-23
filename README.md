# PickSnap Releases

Official public release distribution channel for [PickSnap](https://picksnap.eascivo.com/) by Eascivo Studio.

PickSnap is a local photo culling workspace for macOS and Windows.

## Downloads

Current release: [v1.3.3 — release notes and checksums](https://github.com/eascivo/picksnap-releases/releases/tag/v1.3.3).

| Platform | Architecture | Package |
| :--- | :--- | :--- |
| macOS | Apple Silicon (arm64) | [DMG](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.3/PickSnap-v1.3.3.dmg) |
| Windows | x64 | [Setup EXE](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.3/PickSnap-v1.3.3-Setup.exe) |
| Windows | x64 | [Portable EXE](https://github.com/eascivo/picksnap-releases/releases/download/v1.3.3/PickSnap-v1.3.3-windows-x64.exe) |

The macOS package is ad-hoc signed and not notarized; Windows packages are unsigned. Windows x64 binaries were built and tested under x64 emulation in a Windows 11 ARM64 UTM VM. Intel macOS and physical Windows x64 were not tested.

## What changed in 1.3.3

Safer deletion and save retries preserve consistent photo decisions. Incremental SQLite storage backs up legacy JSON projects before migration. Photo analysis saves completed results individually by default. Model downloads retain TLS and file validation while adding bounded retries, cancellation and persistent recovery controls in all four languages. macOS restores records across /var aliases and uses isolated in-memory storage for private WebKit windows. Windows optional runtimes support deep configuration paths.

The final packages passed local macOS and Windows acceptance. GitHub Actions did not start because of account billing/spending limits; the release owner explicitly approved using the completed local verification for this version.

The corresponding RAW decoder, GCC runtime and Windows OpenBLAS source archives are reused byte-for-byte from 1.3.2 because those libraries are unchanged; their filenames preserve that provenance. See the release notes for validation scope and known limitations, and SHA256SUMS.txt for all six package/source artifacts.

## Official Links

- Official Website: [picksnap.eascivo.com](https://picksnap.eascivo.com/)
- Support & Feedback: support@eascivo.com
- Organization: [Eascivo Studio](https://github.com/eascivo)

---
© 2026 Eascivo. All rights reserved.
