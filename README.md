# ArchCosta Wiki

Welcome to the official documentation for **ArchCosta OS**.

## Introduction

ArchCosta is a professional, performance-tuned distribution based on Arch Linux. It offers a feature-rich desktop experience with multiple desktop environment and window manager options.

## Key Features

- **Multiple Desktop Environments:** XFCE, Cinnamon, MATE, Plasma, GNOME
- **Window Managers:** Hyprland, Sway, Bspwm, Openbox, Wayfire, River, Niri, i3wm
- **Premium Theming:** Auto-generated colors from wallpaper (pywal), dark minimal aesthetic
- **17 Curated Wallpapers:** High-quality 4K wallpapers for all environments
- **Performance Optimized:** Custom kernel tweaks and system optimizations
- **LightDM/SwayDM:** Beautiful login screens with auto-login support
- **Calamares Installer:** Easy installation with guided steps
- **Rolling Release:** Always up-to-date with the latest Arch packages
- **Dracut Support:** Modern initramfs generation for installed systems

## Supported Environments

### Desktop Environments

| DE | Description |
|----|-------------|
| XFCE | Lightweight and fast, ideal for older hardware |
| Cinnamon | Modern desktop with innovative features |
| MATE | Traditional desktop derived from GNOME 2 |
| Plasma | Feature-rich with extensive customization |
| GNOME | Modern, full-featured desktop |

### Window Managers (Wayland)

| WM | Description |
|----|-------------|
| Hyprland | Modern Wayland compositor with rich features |
| Sway | i3-compatible Wayland compositor |
| River | Dynamic tiling compositor |
| Niri | Scrollable-tiling compositor |
| Wayfire | Compositor with 3D effects |

### Window Managers (X11)

| WM | Description |
|----|-------------|
| Bspwm | Minimal floating/tiling window manager |
| Openbox | Highly configurable window manager |
| i3wm | Tiling window manager |

## Installation

### System Requirements

- **CPU:** 64-bit x86 processor
- **RAM:** 2GB minimum (4GB recommended)
- **Storage:** 20GB minimum
- **Graphics:** Any Intel, AMD, or NVIDIA GPU

### Installation Steps

1. Download the latest ArchCosta ISO from GitHub Releases
2. Create a bootable USB using `dd` or Rufus
3. Boot from USB and select ArchCosta
4. The Live environment will load automatically
5. Double-click "Install ArchCosta" on the desktop
6. Follow the Calamares installer steps
7. Choose your preferred desktop environment or window manager
8. Complete the installation and reboot

## Building the ISO

### Build Options

```bash
# Clone the repository
git clone https://github.com/archcosta-os/archcosta.git
cd archcosta

# Build ISO (select DE/WM)
mkarchiso -v -w /tmp/work -o /tmp/out .
```

### Build Flavors

Available in GitHub Actions workflow:
- xfce, plasma, cinnamon, mate, gnome
- hyprland, sway, bspwm, openbox
- wayfire, river, niri, i3wm

## Post-Installation

### Update System
```bash
sudo pacman -Syu
```

### Boot Configuration
```bash
# Regenerate GRUB
sudo grub-mkconfig -o /boot/grub/grub.cfg

# For dracut (if using)
sudo dracut --force --regenerate-all
```

### Network Issues
```bash
sudo systemctl restart NetworkManager
```

## Development

- **GitHub Organization:** https://github.com/archcosta-os
- **Main Repository:** https://github.com/archcosta-os/archcosta
- **Packages (PKGBUILDs):** https://github.com/archcosta-os/archcosta-pkgbuilds
- **Custom Repo:** https://github.com/archcosta-os/archcosta-repo
- **Issue Tracker:** https://github.com/archcosta-os/archcosta/issues

## License

ArchCosta is released under the **GPL-3.0** license.
