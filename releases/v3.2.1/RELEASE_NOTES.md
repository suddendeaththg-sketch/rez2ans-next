# Rez2ANS Next 3.2.1 — Windows compatibility update

This Windows-only maintenance release improves startup reliability on laptops
and desktops with older or unstable integrated graphics drivers, including some
Intel graphics drivers.

## What changed

- The Qt interface now defaults to the Windows WARP software renderer when no
  renderer has been explicitly chosen by the user.
- This avoids the Direct3D 11 driver-initialization failure that can make the
  application appear briefly and then close.
- This setting affects interface drawing only. It does not disable ANSI
  conversion features or prevent advanced users from choosing another Qt
  renderer.

## Install

Run `Rez2ANS-Next-3.2.1-Windows-x64-Setup.exe`. It can be installed over the
previous Windows version. Verify the file with `SHA256SUMS` before installing.

If the application still closes immediately after this update, please report
the Windows version, graphics adapter, driver version, and any Command Prompt
output from launching `rez2ans-next.exe`.
