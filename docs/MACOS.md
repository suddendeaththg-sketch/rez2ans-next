# macOS

Rez2ANS Next has a native macOS DMG packaging path for macOS 12 and newer.
The DMG must be built on a Mac with Xcode Command Line Tools and Qt 6.4 or
newer; it cannot be produced reliably from Linux or Windows.

## Build requirements

- macOS 12 or newer
- Xcode Command Line Tools
- Qt 6 with `macdeployqt` on `PATH`
- CMake

From the Rez2ANS Next source directory, run:

```bash
./build-macos-dmg.sh
```

This builds the application, runs its core tests, bundles the Qt runtime, and
creates `release/Rez2ANS-Next-<version>-macos.dmg`.

## Unsigned distribution

Rez2ANS Next macOS releases are distributed unsigned. This keeps the release
path available without an Apple Developer account, but macOS Gatekeeper will
show a warning the first time the app is opened.

To open an unsigned release, move the app to Applications if desired, then
Control-click the app, choose **Open**, and confirm **Open** in the warning.
After that first approval, it can be opened normally. Users should download
only from the official GitHub Releases page and verify the published checksum.

An unsigned DMG still must be built on macOS; the packaging process uses
Apple's `macdeployqt` and `hdiutil` tools. The first macOS DMG will be listed
on the GitHub Releases page alongside the Windows and Linux downloads.
