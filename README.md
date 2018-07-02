# CHIP-Debian-Kernel

## Disclaimer

This is an un-official Debian 8.0 (Jessie) repository providing Linux kernel, WiFi and 3D driver packages for CHIP.

Use on your own risk.

## Sources

Linux source: https://github.com/kaplan2539/ntc-linux

RTL8723BS driver source: https://github.com/kaplan2539/rtl8723bs

CHIP-Mali driver source: https://github.com/kaplan2539/chip-mali

## Installation

On CHIP run:
```
# Add this repository
wget -qO - https://kaplan2539.github.io/CHIP-Debian-Kernel/PUBLIC.KEY | sudo apt-key add -
echo "deb http://kaplan2539.github.io/CHIP-Debian-Kernel jessie main" | sudo tee --append /etc/apt/sources.list
sudo apt-get update

# Install the new kernel
sudo apt-get install linux-image-4.4.138-chip rtl8723bs-mp-driver-modules-4.4.138 chip-mali-modules-4.4.138
```
