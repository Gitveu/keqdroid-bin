# keqdroid-bin

[![Build and Release](https://github.com/Gitveu/keqdroid-bin/actions/workflows/update.yml/badge.svg)](https://github.com/Gitveu/keqdroid-bin/actions/workflows/update.yml)
[![Upstream Version](https://img.shields.io/github/v/release/Lemonochka/keqdroid?label=upstream&color=blue)](https://github.com/Lemonochka/keqdroid/releases/latest)

Prebuilt Arch Linux binary package for KEQDIS (keqdroid) with automated CI releases.

## Installation

Using `yay` / `paru`:
```bash
yay -U https://github.com/Gitveu/keqdroid-bin/releases/latest/download/keqdroid-bin.pkg.tar.zst
```

Using `pacman`:
```bash
sudo pacman -U https://github.com/Gitveu/keqdroid-bin/releases/latest/download/keqdroid-bin.pkg.tar.zst
```

## Manual Build

```bash
git clone https://github.com/Gitveu/keqdroid-bin.git
cd keqdroid-bin
makepkg -si
```
