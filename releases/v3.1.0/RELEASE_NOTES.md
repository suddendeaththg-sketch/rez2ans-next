# Rez2ANS Next 3.1.0

This release provides the standalone Debian x64 package and Windows x64
installer for Rez2ANS Next, plus portable Linux x64 AppImage and Flatpak
packages.

## Installation

- Debian/Ubuntu/Mint: install `rez2ans-next_3.1.0_amd64.deb` with your
  preferred package installer. It supports Debian 13's Qt package names and
  Ubuntu/Mint's `t64` Qt package names without a compatibility shim.
- Windows: run `Rez2ANS-Next-3.1.0-Windows-x64-Setup.exe`. It installs the
  application under Program Files, adds Start Menu shortcuts, and provides an
  uninstaller through Windows Apps & Features.
- Linux AppImage: mark `Rez2ANS_v3.1-x86_64.AppImage` executable, then run it
  directly. It does not install files into your system.
- Linux Flatpak: install `Rez2ANS-Next-3.1.0-x86_64.flatpak` with `flatpak
  install --user`. The Flatpak is CPU-only and can be slower than the native
  Debian package or AppImage on systems with Vulkan acceleration.

Verify the release files with `SHA256SUMS` before installation.
