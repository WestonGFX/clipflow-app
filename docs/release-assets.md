# Understanding ClipFlow Release Assets

Most users only need one file:

- the `.dmg`

The zipped `.app` is the fallback download if the DMG route is inconvenient or you need a manual support path.

If you are not sure what to pick, choose the `.dmg` and ignore the rest for now.

## Main User Downloads

### `.dmg`

This is the normal Mac install path.

Use this if you just want to install ClipFlow into `Applications`.

### zipped `.app`

This is a fallback artifact.

Use it if:

- the DMG is inconvenient in your environment
- support asks you to try the zip
- you are comparing artifacts manually

## Advanced / Support Artifacts

These files are mainly for verification, support, or advanced users:

### `checksums.txt`

Use this to verify the integrity of the downloaded files.

### `release-manifest.json`

This records the build version, architecture, commit, and release metadata.

### `release-health.json`

This contains packaged runtime measurements like launch timing and app size against budget targets.

### `release-validation.json`

This records release validation results such as artifact correctness and signing/notarization observations.

## What Most People Should Ignore

If you are just trying ClipFlow, you can usually skip:

- `checksums.txt`
- `release-manifest.json`
- `release-health.json`
- `release-validation.json`

Those files exist so support and verification stay honest, not because they are part of the normal install path.

## Why These Files Exist

ClipFlow publishes extra release artifacts because trust and reproducibility matter.

But they are not the normal install path for most users.

If you are just trying the app:

1. download the `.dmg`
2. install it
3. use the install guide if macOS warns about trust or permissions
