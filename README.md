# Spread QEMU images for Ubuntu

This repository contains useful rules to construct QEMU images for Spread.
You can find more about spread at https://github.com/snapcore/spread

## Usage

To use this repository just clone it into `~/.spread/qemu` and run `make`. You
will need to have `make` and `autopkgtest` packages installed.

```shell
mkdir -p ~/.spread/
git clone https://github.com/zyga/spread-qemu-images ~/spread/qemu
```

## Supported images

### Ubuntu

All images provided by https://cloud-images.ubuntu.com/ - most notably LTS
releases, current stable release and the current development release.
