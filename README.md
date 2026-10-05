# Mehdi Mamas

**Software Engineer building AI-powered products, automation systems, and scalable backend infrastructure.**

I build production software across **AI, backend systems, automation, security, and cross-platform applications**.

I am also strong at coding with AI. I use LLMs daily to plan, prompt, review, and ship, and I check the result before it lands.

## Highlights

Pull requests on official SDKs and libraries other people already ship with. Projects I built are listed under Featured Projects.

### Proton Drive CLI Sync — Pull requests

Six pull requests on [proton-drive-cli-sync](https://github.com/lafontaj/proton-drive-cli-sync), two-way Proton Drive sync for Linux.

**Python • pytest • systemd**

- [Test harness](https://github.com/lafontaj/proton-drive-cli-sync/pull/4) stands in for the `proton-drive` CLI so the suite runs without a Proton account. Merged
- [Exit 5](https://github.com/lafontaj/proton-drive-cli-sync/pull/8) when a finished pass still failed an upload, a listing, a trash, or a stall-skip (open)
- [Excluded names](https://github.com/lafontaj/proton-drive-cli-sync/pull/9) already on Drive stay unless the mapping says prune (open)
- [Settings and the CLI](https://github.com/lafontaj/proton-drive-cli-sync/pull/10) are looked up under `~/.config` and on `PATH` (open)
- [Mount re-check](https://github.com/lafontaj/proton-drive-cli-sync/pull/11) before each folder's deletions (open)
- [Mass-deletion guard](https://github.com/lafontaj/proton-drive-cli-sync/pull/12) stays off unless it is turned on (open)

### 🐹 Go MCP SDK — Pull requests

Two pull requests on the [official Go SDK](https://github.com/modelcontextprotocol/go-sdk) for the Model Context Protocol, maintained with Google.

**Go • MCP**

- [Tool.Execution](https://github.com/modelcontextprotocol/go-sdk/pull/1336) keeps the 2025-11-25 `taskSupport` field through a proxy that decodes and re-encodes a tool. `tools/list` sends it only on that protocol version
- [Task type](https://github.com/modelcontextprotocol/go-sdk/pull/1335) adds the tasks extension handle so a task can round-trip (draft). The SDK still does not run a tool as a task

### 🐙 GitHub MCP Server — Pull request

[`watch_workflow_run`](https://github.com/github/github-mcp-server/pull/3406) on [GitHub's official MCP server](https://github.com/github/github-mcp-server). One call waits for an Actions run, sends progress, and stops when the client cancels.

### 💳 ExtPay — Pull request

[Referral codes](https://github.com/Glench/ExtPay/pull/364) for [ExtPay](https://github.com/Glench/ExtPay), the payments library for browser extensions (770+ stars).

### 🔑 iCloudBridge — Pull request

[Ente Auth verification codes](https://github.com/keithvassallomt/icloudbridge/pull/31) matched to existing Apple Passwords logins. Merged.

## What I Build

- 🤖 **AI Systems** — LLM integrations, conversational AI, voice agents, workflow automation
- ⚙️ **Backend Systems** — Node.js, Python, REST APIs, authentication, webhooks, distributed workflows
- 🔐 **Security & Systems** — End-to-end encryption, secure protocols, ephemeral credentials, local networking
- 🧩 **Developer Tooling** — Browser extensions, automation, desktop utilities
- 📱 **Cross-Platform Software** — Web, Electron, React Native, iOS, Android

## Featured Projects

### 🪟 HideMyWindows

Windows app that hides chosen windows from screenshots, recordings, and capture tools. Community continuation of the original by [Cristian Gambino (@zCri)](https://github.com/zCri): same name and purpose, rebuilt from scratch.

**Rust • Tauri 2 • Svelte**

- Hides windows with `SetWindowDisplayAffinity`, matched by process, title, class, or PID, including regex
- Window rules re-apply as new windows appear. Quick launch starts an app already hidden
- Tray, optional start with Windows, and installers for x64, x86, and arm64. The app itself stays visible to capture unless that option is turned on

[View Project](https://github.com/MehdiMamas/HideMyWindows) · [Release v2.0.1](https://github.com/MehdiMamas/HideMyWindows/releases/tag/v2.0.1)

### 🌉 PassBridge

iCloud Passwords in Chrome on macOS and Windows, with an inline menu, a fill shortcut, and a save bar that hands the write to Apple's sheet.

**JavaScript • Chrome Extension • Manifest V3**

- Inline menu on login fields, with keyboard navigation
- Ctrl/Cmd+Shift+L fills and cycles matching logins
- Saving a password hands the write to Apple's own save sheet
- Looks up a password on the page host and on related websites stored with that login
- Loaded unpacked. Apple's helper only accepts its extension id, so there is no Chrome Web Store listing

[View Project](https://github.com/MehdiMamas/open-passwords) · [Release](https://github.com/MehdiMamas/open-passwords/releases/tag/v1.0.1)

Fork of [ManiForoughi2/open-passwords](https://github.com/ManiForoughi2/open-passwords) (Apache-2.0). Apple protocol from [au2001/icloud-passwords-firefox](https://github.com/au2001/icloud-passwords-firefox) (Apache-2.0). Field lists from [bitwarden/clients](https://github.com/bitwarden/clients) (GPL-3.0). Not affiliated with Apple or Bitwarden.

### 🧠 AI Voice Medication Agent

Real-time voice automation system for medication-adherence calls.

**Twilio • Deepgram • ElevenLabs • Node.js**

- Conversational voice workflows
- Real-time speech-to-text and text-to-speech
- Patient-specific call flows
- Voicemail detection and SMS fallback
- Webhook-driven event processing

[View Project](https://github.com/MehdiMamas/DTxPlus-assessment)

### 🔐 ShareGo

End-to-end encrypted sharing between two devices on the same Wi-Fi. One Flutter app for desktop and mobile.

**Flutter • Dart • WebSockets • libsodium**

- Each session uses a new X25519 key. The message key is derived with HKDF-SHA256 and the text is encrypted with XChaCha20-Poly1305
- Keys and messages are wiped when the session ends. Nothing is written to disk
- Windows, macOS, Linux, Android, and iOS

[View Project](https://github.com/MehdiMamas/ShareGo) · [Release v2.0.0](https://github.com/MehdiMamas/ShareGo/releases/tag/v2.0.0)

### 📬 Keytray

Chrome, Edge, and Brave extension that reads verification codes and sign-in links from Gmail. A code can be filled or copied. A link opens only when you choose. Mail stays in the browser on the Gmail readonly scope.

**TypeScript • React • Chrome Extension • Gmail API • OAuth**

- One Gmail account is free. More accounts are a one-time purchase
- Background checks that speed up while a code field is on screen
- Auto-fill for a single box or split digit boxes, plus a Fill chip for recent codes
- Open link for a verification or sign-in URL, only after you click

[View Project](https://github.com/MehdiMamas/multi-gmail-auth-copier) · [Site](https://mehdimamas.dev/gmail-otp-copier/)

### 💸 Minea → Zendrop Cost Finder

Chrome extension that shows Zendrop product cost on a Minea product page, using the Zendrop session already in the browser.

**TypeScript • Chrome Extension • Manifest V3**

- Reads the visible Minea title and searches Zendrop
- Ranks matches with image, cost, and confidence
- Opens the Zendrop product page for the match you pick
- Never asks for or stores an auth token

[View Project](https://github.com/MehdiMamas/minea-zendrop-cost-finder)

### 🎬 Medal On-Device Clip Uploader

Console script that posts every on-device Medal clip from the library, so a local backlog can be uploaded without opening each clip by hand.

**JavaScript • DOM Automation • Browser Console**

- Finds clips still marked on device and skips anything already handled in the run
- Opens the preview, confirms Post, and waits for the upload to finish before closing the dialogs
- Scrolls the library until it stops yielding new clips, then reports uploaded, failed, and elapsed time

[View Project](https://github.com/MehdiMamas/medal-script-to-upload-all-to-unlisted)

### 🎮 SuperPSX Patch Checker

Chrome extension that highlights game versions on SuperPSX when a matching patch exists in the PS-Game-Patch catalog.

**JavaScript • Chrome Extension • Manifest V3**

- Scans version tables for CUSA and PPSA title IDs
- Color-codes 60 FPS patches, other patches, and titles with no match
- Bundled index of 376 title IDs, regenerable from the latest patch release

[View Project](https://github.com/MehdiMamas/superpsx-patch-checker)

### Bitwarden → Apple Keychain

Python script that turns a Bitwarden CSV export into a Chrome import. Safari then imports those passwords into iCloud Keychain. Logins with more than one website are written to a side list so the extra URLs can be added by hand.

**Python**

[View Project](https://github.com/MehdiMamas/bitwarden-to-apple-keychain-converter-script)

## Open Source Contributions

### Proton Drive CLI Sync — Test harness and safer sync

Contributions to [proton-drive-cli-sync](https://github.com/lafontaj/proton-drive-cli-sync). The harness is merged. The safety and path changes are open.

**Python • pytest • systemd**

- A fake `proton-drive` and a pytest suite run with `bash scripts/test.sh` and no Proton account. `PROTON_SYNC_SETTINGS` keeps the suite off the repository settings file
- A finished pass that still failed exits 5. The real-time consumer keeps its markers and waits before retrying that target
- An excluded name already on Drive is trashed by default. A mapping can set `excluded_remote` to `keep`
- Settings move to `~/.config/proton-drive-sync/settings.json`. The CLI is resolved from `PROTON_DRIVE_CLI`, a settings path, a binary next to the scripts, then `PATH`
- Before each folder's deletions the mount is checked again. A refusal stops later deletions in that mapping, and uploads continue
- The mass-deletion guard is off unless configuration turns it on. Thresholds default to 20 items and half the folder

[Pull Request #4](https://github.com/lafontaj/proton-drive-cli-sync/pull/4) (merged) · [#8](https://github.com/lafontaj/proton-drive-cli-sync/pull/8) · [#9](https://github.com/lafontaj/proton-drive-cli-sync/pull/9) · [#10](https://github.com/lafontaj/proton-drive-cli-sync/pull/10) · [#11](https://github.com/lafontaj/proton-drive-cli-sync/pull/11) · [#12](https://github.com/lafontaj/proton-drive-cli-sync/pull/12) (open)

### 🐹 Go MCP SDK — Tool execution field

Added `Tool.Execution` to the [official Go SDK](https://github.com/modelcontextprotocol/go-sdk) so the 2025-11-25 `taskSupport` field survives a proxy that decodes and re-encodes a tool.

**Go • MCP**

- `tools/list` includes `execution` only for protocol version 2025-11-25. A newer list, an older list, and a list with no negotiated version omit it
- `json.Marshal` of a tool still includes the field, so a proxy round-trip keeps it
- The registered tool is copied, not mutated, so one server can show the field to a 2025-11-25 session and hide it from a 2026-07-28 session
- Setting the field does not run the tool as a task

[Pull Request #1336](https://github.com/modelcontextprotocol/go-sdk/pull/1336) (open)

### 🐹 Go MCP SDK — Task type

Added the tasks extension's Task type to the [official Go SDK](https://github.com/modelcontextprotocol/go-sdk), so a task handle can round-trip. Execution stays out: no task methods, and a tool call still does not become a task.

**Go • MCP**

- Task carries taskId, status, statusMessage, createdAt, lastUpdatedAt, ttlMs, and pollIntervalMs
- A nil ttlMs is sent as JSON null, which the extension defines as unlimited
- Task IDs are generated with crypto/rand. Nothing creates a task yet; tests are the only caller

[Pull Request #1335](https://github.com/modelcontextprotocol/go-sdk/pull/1335) (draft)

### 🐙 GitHub MCP Server — Watch workflow runs

Added `watch_workflow_run` to `actions_get` on [GitHub's official MCP server](https://github.com/github/github-mcp-server), so an agent waits for a workflow run in one call instead of polling.

**Go • MCP • GitHub Actions**

- The server polls every 10 seconds, sends progress notifications, and stops as soon as the client cancels
- A timeout returns the live status with `completed: false`. A failed run lists the failed jobs and points to `get_job_logs`

[Pull Request #3406](https://github.com/github/github-mcp-server/pull/3406) (open)

### 🔑 iCloudBridge — Ente Auth verification codes

Match Ente Auth verification codes to existing Apple Passwords logins in [iCloudBridge](https://github.com/keithvassallomt/icloudbridge).

**Python • React • TypeScript**

- Parses a plain-text Ente Auth export and matches each code to an Apple Passwords login by domain, issuer, and username
- Shows a setup key and QR code for Set Up Verification Code, because Apple's importer does not update a login that already exists
- Skips trashed, HOTP, and Steam codes, and leaves ambiguous matches and logins that already have a different code unchanged

[Pull Request #31](https://github.com/keithvassallomt/icloudbridge/pull/31) (merged)

### 💳 ExtPay — Referral codes

Referral code support for [ExtPay](https://github.com/Glench/ExtPay), the payments library for browser extensions (770+ stars).

**JavaScript • Browser Extensions • Stripe**

- Added `extpay.setReferral(code)` and `extpay.getReferral()` to keep a first-touch referral code in extension storage
- Sends the code as `ref` on the existing payment, trial, login, and API-key requests, with no extra network calls
- Wrote a guide for running a referral program on Stripe promotion codes today
- Specified the server-side attribution, rewards, and abuse checks for extensionpay.com

[Pull Request #364](https://github.com/Glench/ExtPay/pull/364) (open)

### 🧩 FitDownloader — Folder destinations and session management

Contribution to [FitDownloader](https://github.com/axel-devs/FitDownloader), a Chrome extension for automated multi-file downloads with configurable concurrency.

**JavaScript • Chrome Extension • Manifest V3 • File System Access API**

- Per-tab destination folders, written through an offscreen document with the File System Access API
- Resolves HTMX landing pages to the direct download link
- Download sessions that survive service worker restarts, with alarms for keep-alive and reconciliation
- Download manager page and a redesigned popup with progress tracking

[Pull Request #1](https://github.com/axel-devs/FitDownloader/pull/1) (open) · [Branch](https://github.com/MehdiMamas/FitDownloader/tree/feature/fs-destination-htmx-resolve)

### 🔊 SoundSwitcher — Device and volume locks

Combined input and output devices in one menu for [SoundSwitcher](https://github.com/creepyLANguy/SoundSwitcher), and added locks so Windows does not change the device or the volume.

**C# • C++ • Windows**

- Lock the Default and Communications roles separately, and lock a device's volume to a chosen level
- The playback helper can set the Default role, the Communications role, or both

[Pull Request #102](https://github.com/creepyLANguy/SoundSwitcher/pull/102) (open)

### Mira Photo — Chat, marketplace, and auth

Merged pull requests on the Mira Photo [frontend](https://github.com/miraphoto/miraphoto-frontend) and [backend](https://github.com/miraphoto/miraphoto-backend).

**TypeScript • Expo • Node.js**

- A centralized chat engine, one thread per model post, and a real-time seen indicator
- Thumbnails, photographer pagination, and fewer round trips on home and marketplace
- Clerk logout in one place, socket auth refresh on reconnect, and optional auth on public user lookups

[Chat engine](https://github.com/miraphoto/miraphoto-frontend/pull/54) · [Seen indicator](https://github.com/miraphoto/miraphoto-frontend/pull/51) · [Home prefetch](https://github.com/miraphoto/miraphoto-frontend/pull/53) · [Socket auth](https://github.com/miraphoto/miraphoto-frontend/pull/60)

## Experience

Software engineering experience spanning:

**AI integrations • Backend architecture • Automation • APIs • Cloud infrastructure • Full-stack applications**

## Tech

**AI:** LLM APIs, Conversational AI, Voice AI, AI Automation, MCP

**AI-assisted coding:** plans, prompts, reviews, and ships with LLMs daily

**Backend:** Node.js, Python, REST APIs, OAuth2, JWT, Webhooks, Microservices

**Frontend:** React, Vue, TypeScript, JavaScript, HTML/CSS, Browser Extensions

**Cloud & DevOps:** AWS, Docker, CI/CD

**Systems & Security:** WebSockets, End-to-End Encryption, Cryptographic Protocols, Local Networking

## Resume

[mehdimamas.github.io/my-resume](https://mehdimamas.github.io/my-resume/)

## Connect

[LinkedIn](https://linkedin.com/in/mehdidev/) · [GitHub](https://github.com/MehdiMamas) · [Website](https://mehdimamas.dev)
