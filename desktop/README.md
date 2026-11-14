# Darkstar Camera Viewer for Windows

[Windows preview 0.8.0-rc.1 release](https://github.com/sacstar/darkstar-camera-viewer-updates/releases/tag/windows-v0.8.0-rc.1)

The single Setup EXE includes the desktop camera runtime, branding, draft terms acceptance and install-folder selection. It adds Ops Center and Admin pages, a latest motion/person clips rail, server health, outage counts, technician HTML reports and credential-free diagnostic JSON. Camera controls stay fixed while the grid scrolls. Existing groups/layouts and encrypted settings transfer remain available.

The optional media tool for stitched MP4 export installs automatically from its upstream distributor on first use; internet is needed for that first media install. No separate Node/browser installation is needed.

App updates checks GitHub Windows releases on startup and every six hours, with manual checking, preview selection, verified download and a user-controlled Install action. It validates repository URLs, product/version, size and SHA-256 and rechecks the file immediately before installation. Windows releases use windows-v tags and windows-update.json; Android/PWA updates are excluded. Windows publication never advances the Android latest release.

The release workflow builds the clean source ZIP, runs updater tests, uploads the EXE and manifest, then performs a real online discovery/download/checksum test. Future reviewed Windows source-package updates trigger this workflow automatically. Release availability depends on that build completing successfully.

Validation before publication: 46 gateway/protocol/storage tests, 5 Windows updater tests and browser fixture checks across 100 grid/sizing/display combinations; alert playback timestamps, health, diagnostics privacy and confirmed camera rename; packaged app launch, monitor bridge, update settings, renderer/gateway crash recovery and settings-preserving manual repair.

Preview limits: unsigned executable; physical multi-monitor/DPI, full installer/silent install and long-running real-site acceptance remain pending. Host reboots/updates were not performed on real Blue Iris servers. Matrix profiles, incident notebooks, vendor-latest checks and AI analysis remain incomplete. Server telemetry is displayed only when reported, and fleet version comparison is not a vendor-latest check. Remote commands require exact-site confirmation and are never replayed automatically after uncertainty.

Keep %APPDATA%/Darkstar Camera Viewer when upgrading. File > Import existing PWA settings copies an original same-account PWA vault without deleting the original. Use encrypted import/export for other devices/accounts.
