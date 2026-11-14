# Darkstar Camera Viewer PWA 0.8.0-rc.1 preview

[Download PWA 0.8.0-rc.1](https://github.com/sacstar/darkstar-camera-viewer-updates/raw/refs/heads/main/pwa/DarkstarCameraViewer-PWA-v0.8.0-rc.1.zip)

The page and camera controls stay fixed while only the camera grid scrolls. This preview also adds Ops Center and Admin navigation, latest motion/person clips with event-time playback, system health where Blue Iris supplies it, outage counts, technician HTML reports and private diagnostic JSON. It retains groups, large layouts, independent monitor windows and encrypted settings transfer.

Extract the complete new ZIP to a separate folder. Run Repair-Darkstar.cmd there, choose Update an existing PWA folder and select your original app folder. The repair tool backs up and preserves the encrypted vault. Refresh existing browser windows after repair. Never delete .local as part of an upgrade.

Validation: 46 automated gateway/protocol/storage tests; browser fixture checks across 100 grid/sizing/display combinations, fixed controls, event playback timestamp, health page, report privacy and confirmed server camera rename. Real host reboots/updates, physical mixed-DPI/multi-monitor and prolonged real-site qualification remain pending. Camera states are server-reported; unknown telemetry stays unknown. Fleet version comparison is not a vendor-latest check. Remote administrative actions require exact-site confirmation and are submitted once; an uncertain result is never replayed automatically.

The Windows software edition has its own startup GitHub updater and installer: [Windows download and instructions](../desktop/README.md). This PWA ZIP still uses the launcher/repair update path. Matrix profiles, incident notebooks and AI analysis remain unfinished. This is a preview, not a production-qualified release.

SHA256: 0d76bbfcad8bf51122cd4443ee327815ac8811faa030d44f69c9ec797ba45f97
