# Rez2ANS Next 3.2.0

Rez2ANS Next 3.2.0 focuses on a clearer, more guided conversion workflow and
more comfortable image preparation.

## Highlights

- Guided quick-start workflow for loading, preparing, converting, and exporting artwork.
- More visible option states for easier day-to-day use.
- Crop selection can be resized from all four sides as well as its corners.
- Improved progress feedback while source-image adjustments are applied.
- Profiles, output-directory support, PNG preview export, and the existing ANSI/BIN export workflow remain available.
- Thread-safe multithreaded conversion and optional Vulkan acceleration remain available in the native desktop packages when supported by the system.

## Packages

- **Windows x64:** Run `Rez2ANS-Next-3.2.0-Windows-x64-Setup.exe`. It installs the application, a Start Menu shortcut, and an uninstaller.
- **Debian/Ubuntu/Mint x64:** Install `rez2ans-next_3.2.0_amd64.deb` with your graphical package installer or `sudo apt install ./rez2ans-next_3.2.0_amd64.deb`.
- **Linux AppImage:** Mark `Rez2ANS-Next-3.2.0-x86_64.AppImage` executable, then run it directly. It is portable and does not install files system-wide.
- **Linux Flatpak:** Install `Rez2ANS-Next-3.2.0-x86_64.flatpak` with `flatpak install --user`. The Flatpak deliberately uses the CPU conversion path, so it can be slower than the Debian package or AppImage on systems where Vulkan is available.

The macOS DMG build path is documented, but an unsigned macOS-built DMG is not
included in this release. See the [macOS guide](../../docs/MACOS.md) for the
one-time Gatekeeper override needed when that package is available.

Verify downloads with the included `SHA256SUMS` file before installing.
