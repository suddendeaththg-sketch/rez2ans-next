# Rez2ANS Next Releases

This repository contains the signed-off release artifacts for Rez2ANS Next.
It is intentionally separate from the application source repository:
`rez2ans-next` contains the source code and build logic, while this repository
contains the distributable packages and GitHub release metadata.

## Current release

`releases/v3.1.0/` contains:

- `rez2ans-next_3.1.0_amd64.deb` — Debian/Ubuntu x64 package
- `Rez2ANS-Next-3.1.0-Windows-x64-Setup.exe` — Windows x64 installer
- `SHA256SUMS` — integrity checks for both files

Verify downloaded files before installing:

```bash
sha256sum -c SHA256SUMS
```

## Publishing to GitHub

After this local repository has been connected to its GitHub remote, pushing a
tag matching the release directory name publishes its artifacts automatically:

```bash
git tag v3.1.0
git push origin main --tags
```

The GitHub Actions workflow creates the GitHub Release and attaches the Debian
package, Windows installer, and checksums. It does not build software or modify
the source repository.
