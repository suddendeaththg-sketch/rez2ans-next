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

## Distribution

Unsigned DMGs may trigger a Gatekeeper warning. For public distribution, sign
the application and DMG with an Apple Developer ID, submit the DMG for Apple
notarization, and staple the result before publishing it.

The first signed and notarized DMG will be listed on the GitHub Releases page
alongside the Windows and Linux downloads.
