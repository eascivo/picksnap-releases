# PickSnap Releases

Official public release distribution channel for [PickSnap](https://picksnap.eascivo.com/) by Eascivo Studio.

PickSnap is a local photo culling workspace for macOS and Windows.

## Downloads

Current release: [v1.4.1 — release notes, checksums and build information](https://github.com/eascivo/picksnap-releases/releases/tag/v1.4.1).

| Platform | Region | Packages |
| :--- | :--- | :--- |
| macOS Apple Silicon (arm64) | China (cn) | [DMG](https://github.com/eascivo/picksnap-releases/releases/download/v1.4.1/PickSnap-v1.4.1-macos-arm64-cn.dmg) · [ZIP](https://github.com/eascivo/picksnap-releases/releases/download/v1.4.1/PickSnap-v1.4.1-macos-arm64-cn.zip) |
| Windows x64 | China (cn) | [Setup EXE](https://github.com/eascivo/picksnap-releases/releases/download/v1.4.1/PickSnap-v1.4.1-windows-x64-cn-Setup.exe) · [ZIP](https://github.com/eascivo/picksnap-releases/releases/download/v1.4.1/PickSnap-v1.4.1-windows-x64-cn.zip) |
| macOS Apple Silicon (arm64) | International (global) | [DMG](https://github.com/eascivo/picksnap-releases/releases/download/v1.4.1/PickSnap-v1.4.1-macos-arm64-global.dmg) · [ZIP](https://github.com/eascivo/picksnap-releases/releases/download/v1.4.1/PickSnap-v1.4.1-macos-arm64-global.zip) |
| Windows x64 | International (global) | [Setup EXE](https://github.com/eascivo/picksnap-releases/releases/download/v1.4.1/PickSnap-v1.4.1-windows-x64-global-Setup.exe) · [ZIP](https://github.com/eascivo/picksnap-releases/releases/download/v1.4.1/PickSnap-v1.4.1-windows-x64-global.zip) |

The two compatibility filenames used by older in-app updaters contain the exact global-package bytes: `PickSnap-v1.4.1.dmg` and `PickSnap-v1.4.1-Setup.exe`.

The macOS package is ad-hoc signed and not notarized; Windows packages are unsigned. Windows x64 binaries were built and tested under x64 emulation in a Windows 11 ARM64 UTM VM. Intel macOS and physical Windows x64 were not tested.

## What changed in 1.4.1

Sort photos by capture time, filename, rating or score; select multiple photos and set or clear ratings with undo; export selected photos; and import RAW files only, with normal-import fallback when no RAW files are present. Search-model downloads and the anonymous usage statistics client also receive fixes. See [the full bilingual release notes](releases/v1.4.1.md).

Photo processing stays on your computer and original files remain unchanged. Search models use hf-mirror in cn packages and Hugging Face in global packages; providers may redirect downloads to their CDNs. Initial model downloads require internet access. Anonymous statistics remain optional and can be disabled.

## Checksums and third-party sources

Verify downloads with `SHA256SUMS.txt` in the release assets. The build manifest distinguishes the frozen package source from the final merge and records the accepted QA limitations.

The current decoder uses [rawpy 0.27.1](https://github.com/letmaik/rawpy/tree/a39c2e7a44911889c3360891012f862f904ba551) and its pinned [LibRaw sources](https://github.com/letmaik/rawpy/tree/v0.27.1/external). Windows uses the upstream rawpy wheel. macOS uses 0.27.1+psomp1 with OpenMP enabled, LibRaw 0.22.1 and [LLVM OpenMP 21.1.8](https://github.com/llvm/llvm-project/tree/llvmorg-21.1.8/openmp); codec sources and build settings follow [the pinned upstream recipe](https://github.com/letmaik/rawpy/blob/v0.27.1/.github/scripts/build-macos.sh). Bundled notices retain the applicable licenses. Corresponding source and build-instruction requests can be sent to support@eascivo.com.

Historical source archives remain available with their original filenames in [v1.4.0](https://github.com/eascivo/picksnap-releases/releases/tag/v1.4.0): [RAW decoder](https://github.com/eascivo/picksnap-releases/releases/download/v1.4.0/PickSnap-v1.3.2-RAW-decoder-sources.tar.gz), [GCC runtime](https://github.com/eascivo/picksnap-releases/releases/download/v1.4.0/PickSnap-v1.3.2-GCC-runtime-sources.tar.gz), and [Windows OpenBLAS](https://github.com/eascivo/picksnap-releases/releases/download/v1.4.0/PickSnap-v1.3.2-Windows-OpenBLAS-sources.tar.gz). Their historical names alone do not certify them as a complete source archive for every 1.4.1 dependency. No new source archives are attached to this release.

## Official Links

- Official Website: [picksnap.eascivo.com](https://picksnap.eascivo.com/)
- Support & Feedback: support@eascivo.com
- Organization: [Eascivo Studio](https://github.com/eascivo)

---
© 2026 Eascivo. All rights reserved.
