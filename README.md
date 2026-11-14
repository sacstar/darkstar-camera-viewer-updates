# Darkstar Camera Viewer updates

Public Android release files for Darkstar Camera Viewer. This repository contains app installers, an update manifest and release notes. It does not contain saved sites, camera credentials, signing keys, camera recordings or private configuration.

## Install and update

Open the latest release and install the regular Darkstar Camera Viewer APK. Users of v0.5.1 need one manual installation of the latest APK to add the updater. Keep the existing app installed so its sites and settings remain in place.

After that, the app automatically checks GitHub when opening/resuming, at most once every six hours. Settings → App updates also provides Check for updates, Download update and Install update. Android asks for installation permission and confirmation. The app verifies the APK's checksum, package, version and signing certificate before opening the installer.

The default update feed is:

https://github.com/sacstar/darkstar-camera-viewer-updates/releases/latest/download/latest.json

## Restore a previous version

Settings → App updates → Restore previous version uses the published recovery build. Android normally blocks installing a lower internal version over a newer one, so recovery packages contain the previous working camera code with a higher installation version code and keep the updater installed. Do not uninstall the app to roll back.

The initial recovery package is based on the stable v0.5.1 camera source, with the updater retained. Its camera feature set matches the initial v0.6.0 release, which introduces update management.

## Release channel

The main v0.6.1 build uses versionCode 15. Its recovery build uses versionCode 16 and restores v0.6.0 camera code. The v1.0.0-rc.4 production candidate reserves versionCode 23 and recovery code 24. Future main releases must use versionCode 25 or higher and reserve a higher code for their recovery package. Only repository maintainers can publish releases. Users receive update files; they do not gain publishing access.

This is private-distribution Android software hosted through a public release repository, not a Google Play listing. The APKs are publicly downloadable. Camera access still requires the user's own Blue Iris server address, account and network access.

## Private production candidate

v1.0.0-rc.4 is prepared as a non-debuggable release build for private GitHub/OneDrive distribution. It retains the existing signing identity for in-place upgrades and includes unique backup filenames plus a circular PTZ pad. PTZ controls and movement requests require explicit per-camera Blue Iris PTZ support; fixed, unknown-capability and disabled cameras are excluded. The PTZ pad starts hidden for every camera; use the toolbar to open it and Hide controls to close it. Its higher-code recovery restores rc.3 camera code while retaining the new updater.

Candidates are marked as pre-releases and do not advance the stable update feed. Physical phone, all-site and extended-use acceptance are required before promotion. Google Play publication is not part of this distribution path.


## Choose update channels and versions

The new App updates screen has Stable, Preview and Custom channels, a published-version chooser, release notes and clear download/install/recovery actions. Preview includes published pre-releases and automatically checks future candidates; Stable excludes pre-releases. Release-candidate builds default to Preview for this repository. APK signature, package, version and checksum checks still apply. Older builds cannot be installed directly over higher installation codes; use a compatible signed recovery.

Publication status: v1.0.0-rc.4 is prepared and saved as a draft. Its GitHub APK assets and manifest are not yet published; the address below will become usable after publication.

Older installed updaters need one update to receive this menu. In their existing update-address field, enter:

https://github.com/sacstar/darkstar-camera-viewer-updates/releases/download/v1.0.0-rc.4/latest.json

Then choose Check for updates, Download update and Install update. Keep the existing app installed. After updating, choose Preview to track later candidates. The recovery preserves the new updater while restoring rc.3 camera code.
