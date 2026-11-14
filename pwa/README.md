# Darkstar Camera Viewer PWA v0.6.0

[Download PWA ZIP (source and built app)](https://github.com/sacstar/darkstar-camera-viewer-updates/raw/refs/heads/main/pwa/DarkstarCameraViewer-PWA-v0.6.0.zip)

Open a saved view and choose Arrange. Drag camera handles with mouse or touch, then Save layout. Arrow keys and Home/End also move cameras; Escape cancels a drag. Edge dragging scrolls the grid. Cancel arrangement restores the original order. Save as new layout creates an independent named copy.

Create layout opens a visual editor: choose up to 36 cameras across sites and 1–6 visible rows/columns. Up to 50 named views are supported. Existing backups and viewport-only previews remain compatible.

New installation: extract and run Setup-Darkstar.cmd. Update: stop the old gateway, copy the release contents into its existing PWA folder, KEEP the .local folder/vault.json, then run Start-Darkstar.cmd and refresh the browser.

This is a Windows local-gateway PWA bound to 127.0.0.1, not a public camera website. The ZIP contains source and built files, no saved sites/credentials/recordings.

Validation: production build and 38 Node tests passed. Chrome browser checks passed for mouse/touch drag, keyboard moves, edge scrolling/Escape, Save/Cancel, custom copies, reload persistence and unsaved-navigation protection on synthetic two-site streams. Physical touch hardware and new real-site checks were not performed for this change.

ZIP SHA256: `65b537db5dc79a8572ff5db95621bd296fc894f7d4a6928ae453536b7c727385`
