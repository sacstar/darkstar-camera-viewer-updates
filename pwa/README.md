# Darkstar Camera Viewer PWA v0.7.1

[Download PWA v0.7.1](https://github.com/sacstar/darkstar-camera-viewer-updates/raw/refs/heads/main/pwa/DarkstarCameraViewer-PWA-v0.7.1.zip)

The app header and camera-wall toolbar now show the version. The launcher detects an older running gateway and directs you to Repair-Darkstar.cmd rather than silently opening old features.

Extract the complete new ZIP into a separate folder. Run Repair-Darkstar.cmd there, choose Update an existing PWA folder, and select your original app folder. It makes a dated encrypted-vault backup, replaces app files and restarts the gateway while preserving saved sites, groups and layouts. Alternatively choose Restart this folder. Unrelated services are not stopped. Refresh the browser after repair.

Retains the Darkstar Technical logo, layouts with up to 1,000 cameras, 64/81/100/144-pane grids, named cross-site groups, drag ordering and independent monitor windows with auto-fit and camera-wall mode. Groups are included in encrypted settings backups. Optional browser monitor placement requires permission; manual placement remains available. The Windows software edition can use native monitor discovery.

Validation: 43 automated tests passed; browser checks passed for visible version, 120-camera layouts/groups, reload persistence, independent monitor windows, fullscreen and permission fallback. An actual running v0.6.1 gateway was upgraded to v0.7.1; the encrypted vault stayed byte-for-byte unchanged and its saved group remained readable. Repair rejected an unrelated local HTTP service without stopping it. These checks used isolated test settings. Physical multi-monitor/DPI qualification and prolonged real-site testing remain pending.

The expanded operations/health dashboard and administration features remain under development and are not included in this package. This is a Windows local-gateway PWA, not a hosted public dashboard. No private settings or camera credentials are included.

SHA256: c4f695a2f4b6fc6f6d977f9e803dffe8b057864a85842756ba66d47254d9ccea
