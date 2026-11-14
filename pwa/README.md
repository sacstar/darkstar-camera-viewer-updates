# Darkstar Camera Viewer PWA v0.6.1

[Download PWA ZIP (source and built app)](https://github.com/sacstar/darkstar-camera-viewer-updates/raw/refs/heads/main/pwa/DarkstarCameraViewer-PWA-v0.6.1.zip)

Open a saved view and choose Arrange. Drag camera handles with mouse or touch, then Save layout. Arrow keys and Home/End also move cameras; Escape cancels a drag. Edge dragging scrolls the grid. Cancel arrangement restores the original order. Save as new layout creates an independent named copy.

Create layout opens a visual editor: choose up to 36 cameras across sites and 1–6 visible rows/columns. Up to 50 named views are supported. Existing backups and viewport-only previews remain compatible.

New installation: extract and run Setup-Darkstar.cmd. Update from 0.6.0: first copy the release contents into the existing PWA folder, KEEP .local/vault.json, then run the corrected Stop-Darkstar.cmd followed by Start-Darkstar.cmd and refresh the browser.

This is a Windows local-gateway PWA bound to 127.0.0.1, not a public camera website. The ZIP contains source and built files, no saved sites/credentials/recordings.

Validation: production build and 40 Node tests passed. Chrome browser checks passed for mouse/touch drag, keyboard moves, edge scrolling/Escape, Save/Cancel, custom copies, reload persistence and unsaved-navigation protection on synthetic two-site streams. Physical touch hardware and new real-site checks were not performed for this change.

ZIP SHA256: `c5a16f2518e13d8b8a611e0c335102b989a1c793df1754818a42cb9ef6919ea1`


Startup fix: launcher and Stop shortcut previously recognized only gateway versions 0.1–0.5. Version 0.6.0 could start successfully but still report failure. Version 0.6.1 recognizes current/future version headers. First launch, repeated launch without a duplicate server, and Windows bootstrap Stop were verified on a clean installation using a dedicated test port.
