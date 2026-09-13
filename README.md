# WR-AI for Windows

WR-AI is a local-first personal AI workspace for reading documents, discussing their contents, and saving and retrieving information. Qwen performs the reasoning locally; tools extract document text into the conversation context and operate the internal saved workspace.

## Download and install

**[Download WR-AI 1.0.3 Installer](https://github.com/waaa3999-cmyk/WR-AI-Releases/releases/download/wr-ai-1.0.3-096A123-release.10/WR-AI-Download-Installer.exe)** | [Release details and checksums](https://github.com/waaa3999-cmyk/WR-AI-Releases/releases/tag/wr-ai-1.0.3-096A123-release.10)

Open the release and choose **WR-AI-Download-Installer.exe**. It downloads the payload automatically, resumes interrupted downloads, and verifies the sizes and SHA-256 hashes before opening Direct Setup. Review the EULA and installation options. You do not need to join the numbered payload parts manually.

This repository contains distribution documentation only. Compiled application downloads are stored in GitHub Releases, not in repository source files.

## System requirements

- Windows 10 build 19041 or later, or Windows 11, x64.
- At least 28 GiB visible RAM; 32 GB installed RAM is recommended.
- A compatible NVIDIA CUDA GPU with at least 4 GB VRAM and an appropriate driver.
- Microsoft Edge WebView2 Runtime.
- At least 60 GiB free space during download/installation and 35 GiB for ongoing application/model storage, plus your documents.

Local AI use does not need an activation key, paid API, or continuous internet connection. The initial download requires internet access. CPU-only operation has not been accepted for this release. Performance and OCR accuracy vary with the computer and input; review important extracted figures.

## Language and privacy

New installations start in English. Arabic and RTL presentation remain available in Settings. Qwen responds in the user's language. Updates are designed to preserve user data; keep your own backups of important documents.

## Integrity and licenses

Read the exact release's signing warning, verification status, requirements, and SHA-256 information before installation. Download only from this repository's official releases.

Each release includes the WR-AI EULA, Gemma notices and terms, production SBOM, THIRD_PARTY_NOTICES, license-file manifest, and checksum information. Gemma's terms and prohibited-use policy apply. WR-AI source code, private credentials/keys, production databases, user files, logs, checkpoints, and development environments are not distributed.

Official website: [getwrai.com](https://getwrai.com/).

For the update details and known limitations, read the [1.0.3 release notes](https://github.com/waaa3999-cmyk/WR-AI-Releases/releases/tag/wr-ai-1.0.3-096A123-release.10).
