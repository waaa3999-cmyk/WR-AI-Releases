# WR-AI Privacy Policy

Effective September 5, 2026. This policy applies to WR-AI 1.0.0 Direct build
`096A122-release.1` and WR-AI 1.0.1 Microsoft Store build
`096A122-store.2`.

WR-AI processes conversations and files locally on the user's Windows device.
Core AI features do not transmit chat text or file contents to a cloud AI
service. Application services bind to localhost, and Meilisearch analytics are
disabled in the production runtime configuration. The application does not
download replacement executable code.

WR-AI stores conversations, uploaded files, indexes, revisions, and settings in
a user-data directory outside the installed program directory. The Direct
distribution uses `%LOCALAPPDATA%\WR-AI`; the Microsoft Store distribution uses
`%USERPROFILE%\WR-AI Data`. Updates preserve these directories. Uninstallers
intentionally retain them to avoid deleting user-created work. Users may delete
the applicable directory separately when they no longer need their data.

The GitHub Download Installer retrieves public release assets from the official
[WR-AI Releases repository](https://github.com/waaa3999-cmyk/WR-AI-Releases)
and writes a build-specific download, staging, bootstrap, and diagnostic-log
cache under `%LOCALAPPDATA%\WR-AI-InstallerCache`.
After Direct Setup reports a successful installation, the downloader removes
the build-specific cache and bootstrap. If a download is interrupted or
installation fails, it retains the verified cache and transcript so the
operation can resume or be diagnosed; the user may remove that installer cache
separately when it is no longer needed.

The redacted diagnostic export omits conversation text, file contents, file
names, absolute paths, and raw hardware identifiers. Direct automatic updates
are disabled in this release. GitHub hosts the public Direct-release files and
may separately process repository access and release-download activity under
GitHub's own terms and privacy policy. GitHub is a distribution channel for
the Direct release; it is not the WR-AI privacy, support, or AI-output-report
contact channel.

Data controller: WR-AI, published by wrai.
Privacy questions, support requests, and AI-output reports:
[WR-AI contact and reporting page](https://getwrai.com/contact).

The Microsoft Store build provides a report action beside completed AI
responses. After an explicit confirmation, it opens the WR-AI contact and
reporting page in the user's default browser. The desktop application does not
prefill, attach, or automatically transmit the conversation, prompt, response,
or files. The contact page is a separate web interaction. The user decides
whether to submit a report and what information to include. If the user submits
the form, only the information the user chooses to enter is sent through that
web page.

Microsoft separately processes Store acquisition, download, update, crash, and
commerce data according to Microsoft's policies. WR-AI does not receive chat or
file content through that Store activity.
