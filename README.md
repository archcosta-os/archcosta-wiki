# ArchCosta Wiki

Welcome to the official documentation for **ArchCosta OS**.

## Introduction

ArchCosta is a professional, performance-tuned distribution based on Arch Linux. It is designed for low-end systems while providing a feature-rich desktop experience with multiple desktop environment options.

## Key Features

- **Multiple Desktop Environments:** Choose from Cinnamon, XFCE, MATE, or Plasma
- **Performance Optimized:** Custom kernel tweaks and system optimizations
- **LightDM Greeter:** Beautiful login screen with auto-login support
- **Calamares Installer:** Easy installation with guided steps
- **Rolling Release:** Always up-to-date with the latest Arch packages

## Supported Desktop Environments

### Cinnamon
A modern desktop featuring a traditional layout with an innovative window list applet.

### XFCE
A lightweight and fast desktop environment ideal for older hardware.

### MATE
A traditional desktop environment derived from GNOME 2.

### Plasma (KDE)
A feature-rich desktop with modern aesthetics and extensive customization.

## Installation

### System Requirements

- **CPU:** 64-bit x86 processor
- **RAM:** 2GB minimum (4GB recommended)
- **Storage:** 20GB minimum
- **Graphics:** Any Intel, AMD, or NVIDIA GPU

### Installation Steps

1. Download the latest ArchCosta ISO
2. Create a bootable USB using dd or Rufus
3. Boot from USB and select "ArchCosta Linux (Standard)"
4. The Live environment will load automatically
5. Double-click "Install ArchCosta" on the desktop
6. Follow the Calamares installer steps
7. Choose your preferred desktop environment
8. Complete the installation and reboot

## Desktop Environment Selection

During installation, you can choose from:

- **ArchCosta Cinnamon** - Modern and innovative
- **ArchCosta XFCE** - Lightweight and fast
- **ArchCosta MATE** - Traditional and stable
- **ArchCosta Plasma** - Feature-rich and customizable

## Post-Installation

### Update System
```bash
sudo pacman -Syu
```

### Install AUR Helper (Optional)
```bash
# Install yay
sudo pacman -S yay
```

### Install Drivers

**NVIDIA:**
```bash
sudo pacman -S nvidia nvidia-utils
```

**AMD:**
```bash
sudo pacam -S xf86-video-amdgpu
```

## Troubleshooting

### No Sound
```bash
# Install pipewire
sudo pacman -S pipewire pipewire-alsa pipewire-pulse
```

### Network Issues
```bash
# Restart NetworkManager
sudo systemctl restart NetworkManager
```

## Development

- **GitHub Organization:** https://github.com/archcosta-os
- **Main Repository:** https://github.com/archcosta-os/archcosta
- **Packages Repository:** https://github.com/archcosta-os/archcosta-pkgbuilds
- **Issue Tracker:** https://github.com/archcosta-os/archcosta/issues
- **Wiki:** https://github.com/archcosta-os/archcosta-wiki

## License

ArchCosta is released under the **GPL-3.0** license.
