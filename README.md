# WR-AI for Windows

This repository is the official binary distribution channel for WR-AI, a local-first desktop AI assistant for Windows. WR-AI 1.0.0 build `096A122-release.1` assets contain the compiled application, local AI models, runtime components, license notices, and integrity manifests. They exclude the WR-AI desktop application's Python, TypeScript/TSX, and Rust source trees, source maps, tests, user files, production databases, logs, checkpoints, private keys, credentials, and development environments. The small Download Installer necessarily embeds a reviewed PowerShell downloader resource and its release manifest; those bootstrap resources perform download and verification and are separate from the WR-AI desktop application source tree. Third-party source-form material required by a component license is identified in the SBOM and license inventory.

## Download and install

1. Open the [latest WR-AI release](https://github.com/waaa3999-cmyk/WR-AI-Releases/releases/latest).
2. Download **WR-AI-Download-Installer.exe**.
3. Run the Download Installer, review and accept the WR-AI EULA before payload download begins, and follow the English installer interface. It resumes interrupted downloads, verifies the size and SHA-256 of every part, reconstructs the verified payload, and starts Direct Setup only after verification succeeds. After Direct Setup reports success, it removes the build-specific download, staging, and bootstrap cache. If download or installation fails, the cache and transcript are retained for resume or diagnosis.

The application payload is split into Release assets no larger than 1900 MiB (1,992,294,400 bytes) each. You do not need to download or join those parts manually when using the Download Installer; it performs the size and SHA-256 checks automatically.

## System requirements

- Windows 10 version 2004 (build 19041) or later, or Windows 11; x64 only.
- 32 GB RAM recommended, with at least 28 GiB of visible physical memory.
- A current NVIDIA GPU with at least 4 GB VRAM. The tested baseline is an NVIDIA GeForce RTX 2050 4 GB.
- Microsoft Edge WebView2 Runtime.
- At least 60 GiB of free disk space during download, verification, and installation; retain at least 35 GiB afterward for WR-AI, indexes, revisions, temporary extraction, and user files.

This release does not claim a tested CPU-only or non-NVIDIA fallback.

## Language and privacy

English is the default interface language for a new installation. Arabic remains available in Settings with full right-to-left layout support. The local Qwen model responds in the language used by the user; the interface language does not force model responses into English.

Core chat, document, OCR, search, and model processing run locally. User conversations and files remain in the local WR-AI data directory. Network access is used by the small download installer only to retrieve public release assets from this GitHub repository.

## Integrity and licenses

Build `096A122-release.1` is distributed without Authenticode signatures. Windows may show Unknown Publisher or Microsoft Defender SmartScreen warnings. Download only from this official repository, verify the published SHA-256 values, and continue only if you accept the risk of running unsigned installers.

Each release includes `SHA256SUMS-GITHUB.txt`, `WR-AI-GitHub-Assets.json`, a CycloneDX production SBOM, the WR-AI EULA, Gemma terms and notice, and `THIRD_PARTY_NOTICES.txt` as the generated notice and attribution index. Complete copied license and model-term files are installed in the payload's `licenses` directory and mapped by `LICENSE_FILE_MANIFEST.json`. Verify that the release tag, asset sizes, and checksums match the files you downloaded.

Support and release questions: use the repository [Issues](https://github.com/waaa3999-cmyk/WR-AI-Releases/issues) page.
