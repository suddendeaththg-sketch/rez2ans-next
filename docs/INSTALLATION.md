# Installation

## Windows x64

1. Download `Rez2ANS-Next-3.1.0-Windows-x64-Setup.exe` from the current release folder or GitHub Release.
2. Optionally verify it against `SHA256SUMS`.
3. Run the installer and follow the prompts.
4. Launch **Rez2ANS Next** from the Start Menu.

The installer places the application in Program Files, adds an Apps & Features entry, and includes an uninstaller.

## Debian and Ubuntu x64

Download `rez2ans-next_3.1.0_amd64.deb`, then install it with your graphical package installer or from a terminal:

```bash
sudo apt install ./rez2ans-next_3.1.0_amd64.deb
```

If your system reports missing dependencies, run:

```bash
sudo apt --fix-broken install
```

Launch Rez2ANS Next from your applications menu after installation.

## Vulkan acceleration

Vulkan is optional. When a compatible GPU and driver are available, Rez2ANS Next can offer its Vulkan-accelerated path. The normal CPU path remains available and does not require a discrete NVIDIA card.

Keep your graphics driver current. If a Vulkan option is unavailable or causes problems, use the CPU path and include your GPU and driver details when asking for help.

## Updating

Install a newer release over an older one using the same platform installer. Keep any profiles or export folders you want to preserve before uninstalling.
