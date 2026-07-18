# Rez2ANS Next 3.2.2 — Windows startup fix

This Windows-only maintenance release replaces the 3.2.1 Windows update.

## Fixed

- The installer now explicitly configures the bundled Qt QML module directory.
- Fixes startup errors such as:

  ```text
  module "QtQuick.Controls" plugin "qtquickcontrols2plugin" not found
  ```

- Retains the safer Windows WARP interface-rendering default for systems with
  older or unstable integrated graphics drivers.

## Install

Run `Rez2ANS-Next-3.2.2-Windows-x64-Setup.exe`. It can be installed over any
previous Windows version. Verify the file with `SHA256SUMS` before installing.
