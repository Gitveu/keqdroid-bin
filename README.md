# keqdroid-bin

[![Check for upstream update](https://github.com/Gitveu/keqdroid-bin/actions/workflows/update.yml/badge.svg)](https://github.com/Gitveu/keqdroid-bin/actions/workflows/update.yml)
[![Upstream Version](https://img.shields.io/github/v/release/Lemonochka/keqdroid?label=upstream&color=blue)](https://github.com/Lemonochka/keqdroid/releases/latest)
[![Package Version](https://img.shields.io/github/v/release/Gitveu/keqdroid-bin?label=package&color=green)](https://github.com/Gitveu/keqdroid-bin/releases/latest)

Prebuilt Arch Linux binary package for Keqdroid.

## Installation

### Option 1: Prebuilt binary (Recommended)

```bash
curl -LO https://github.com/Gitveu/keqdroid-bin/releases/latest/download/keqdroid-bin.pkg.tar.zst
sudo pacman -U keqdroid-bin.pkg.tar.zst
```

### Option 2: Build from source

```bash
git clone https://github.com/Gitveu/keqdroid-bin.git
cd keqdroid-bin
makepkg -si
```

## Removal

```bash
sudo pacman -R keqdroid-bin
```
