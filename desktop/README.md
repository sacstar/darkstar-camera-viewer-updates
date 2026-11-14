# Recovery and offline settings export 0.8.2-rc.1

[Download Windows recovery preview](https://github.com/sacstar/darkstar-camera-viewer-updates/releases/tag/windows-v0.8.2-rc.1)

File > Export sites and settings opens a native backup flow independent of the gateway. Press Alt to show File if needed. Choose sites, enter and confirm a backup passphrase locally, and choose where to save the encrypted portable backup. The original vault is read only and preserved. Run this on the computer and Windows account that owns the original settings. The recovery page also offers this export when the gateway is unavailable, including startup failures.

This preview records the previously missing redacted gateway exception details in gateway-fatal.jsonl. It provides restart, diagnostic-folder, backup and update actions on a recovery page instead of leaving only a blank camera window. Startup update checks and the 0.8.1 authentication hold are retained.

The reported exit-code-1 crash has NOT been identified or confirmed fixed. This is a recovery/diagnostic build so settings can be backed up and the missing exception captured. No live Blue Iris login probes were used. Validation includes 10 authentication/updater/report tests, offline native export with a stopped gateway and with an occupied startup port, unchanged-vault verification, and a nine-host packaged fixture run with socket resets/stalls/permission errors. The actual crash was not reproduced. Sidebar redesign and additional features remain separate work until the failure is understood.

# Authentication hotfix 0.8.1-rc.1

[Download the Windows authentication hotfix](https://github.com/sacstar/darkstar-camera-viewer-updates/releases/tag/windows-v0.8.1-rc.1)

Fixes automatic authentication retry paths that can contribute to Blue Iris IP bans. One rejected or uncertain credentialed login pauses this site's authentication across previews, streams, background reads and LAN/WAN routes. The encrypted hold survives app/gateway restart; Refresh does not bypass it. HTTP 403, unexpected media content and permission-rejected non-camera-list commands no longer trigger fresh logins. Credentialed login responses are never replayed after a transport error. Session renewal is bounded.

Retains startup GitHub update checks. Review the affected site's login and Blue Iris ban status, then explicitly save its connection settings to allow one new attempt. Keep auto-ban protection enabled. The exact cause and affected sites still require Blue Iris Connections/Messages logs; development did not send live host login probes. Nine authentication/updater fixture tests passed. The sidebar redesign is being developed separately.

# Darkstar Camera Viewer for Windows

[Windows preview 0.8.0-rc.1 release](https://github.com/sacstar/darkstar-camera-viewer-updates/releases/tag/windows-v0.8.0-rc.1)

The single Setup EXE includes the desktop camera runtime, branding, draft terms acceptance and install-folder selection. It adds Ops Center and Admin pages, a latest motion/person clips rail, server health, outage counts, technician HTML reports and credential-free diagnostic JSON. Camera controls stay fixed while the grid scrolls. Existing groups/layouts and encrypted settings transfer remain available.

The optional media tool for stitched MP4 export installs automatically from its upstream distributor on first use; internet is needed for that first media install. No separate Node/browser installation is needed.

App updates checks GitHub Windows releases on startup and every six hours, with manual checking, preview selection, verified download and a user-controlled Install action. It validates repository URLs, product/version, size and SHA-256 and rechecks the file immediately before installation. Windows releases use windows-v tags and windows-update.json; Android/PWA updates are excluded. Windows publication never advances the Android latest release.

The release workflow builds the clean source ZIP, runs updater tests, uploads the EXE and manifest, then performs a real online discovery/download/checksum test. Future reviewed Windows source-package updates trigger this workflow automatically. Release availability depends on that build completing successfully.

Validation before publication: 46 gateway/protocol/storage tests, 5 Windows updater tests and browser fixture checks across 100 grid/sizing/display combinations; alert playback timestamps, health, diagnostics privacy and confirmed camera rename; packaged app launch, monitor bridge, update settings, renderer/gateway crash recovery and settings-preserving manual repair.

Preview limits: unsigned executable; physical multi-monitor/DPI, full installer/silent install and long-running real-site acceptance remain pending. Host reboots/updates were not performed on real Blue Iris servers. Matrix profiles, incident notebooks, vendor-latest checks and AI analysis remain incomplete. Server telemetry is displayed only when reported, and fleet version comparison is not a vendor-latest check. Remote commands require exact-site confirmation and are never replayed automatically after uncertainty.

Keep %APPDATA%/Darkstar Camera Viewer when upgrading. File > Import existing PWA settings copies an original same-account PWA vault without deleting the original. Use encrypted import/export for other devices/accounts.
