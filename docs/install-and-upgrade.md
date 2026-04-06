# ClipFlow Beta Install And Upgrade Guide

## Download

Download the latest beta build from:

- [ClipFlow releases](https://github.com/WestonGFX/clipflow-app/releases)

Look for:

- `.dmg`
- zipped `.app`
- `checksums.txt`
- `release-manifest.json`

## Install Paths

### Signed / notarized release

If the beta release is Developer ID signed and notarized:

1. Open the DMG.
2. Drag `ClipFlow.app` into `Applications`.
3. Launch ClipFlow normally.

### Unsigned or ad-hoc beta build

Some beta builds may still be structurally valid but not notarized yet.

Try the normal macOS override flow first:

1. Move `ClipFlow.app` into `Applications`.
2. Right-click the app and choose `Open`.
3. Confirm the warning if macOS offers the override path.

If Gatekeeper still blocks the build and you trust the beta, use this local workaround:

```bash
codesign --force --deep --sign - /Applications/ClipFlow.app
xattr -dr com.apple.quarantine /Applications/ClipFlow.app
```

This is a local testing workaround only. It does not replace proper Developer ID signing and notarization for public distribution.

## Upgrade Behavior

ClipFlow stores data in:

- `~/Library/Application Support/com.clipflow`

Upgrades preserve:

- clipboard history
- snippets
- settings
- diagnostics state
- recovery metadata

## Migration From The Old Electron Build

The old Electron app used a different bundle/app support path:

- app name: `Clipflow.app`
- legacy support path: `~/Library/Application Support/com.clipflow.app`

The current Tauri app is:

- app name: `ClipFlow.app`
- support path: `~/Library/Application Support/com.clipflow`

ClipFlow migrates legacy support files forward without overwriting newer data already present in the current support directory.

## Uninstall Or Reset

To uninstall:

1. Delete `ClipFlow.app` from `Applications`.
2. Remove the support directory if you want to clear all local data:

```bash
rm -rf ~/Library/Application\ Support/com.clipflow
```

## Reporting Beta Problems

Please include:

- ClipFlow version
- macOS version
- which asset you installed
- whether the build was signed/notarized or required the local workaround
- diagnostics copied from Settings when possible
