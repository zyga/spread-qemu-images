# Spread QEMU images for Ubuntu

This repository contains useful rules to construct QEMU images for Spread.
You can find more about spread at https://github.com/snapcore/spread

## Installation

To use this repository just clone it into `~/.spread/qemu` and run `make`. You
will need to have `make`, `autopkgtest`, `qemu-system-x86` and `genisoimage`
packages installed.

**IMPORTANT** you really have to get `autopkgtest` from the
`-backports` repository, the main repository contains an old and
broken version that doesn't work.

Installation instructions distilled:

```shell
. /etc/os-release
apt-get install make qemu-system-x86 genisoimage
apt-get install install -t ${VERSION_CODENAME}-backports autopkgtest
mkdir -p ~/.spread/
git clone https://github.com/zyga/spread-qemu-images ~/spread/qemu
make -C ~/spread/qemu
```

## Supported images

### Ubuntu

All images provided by https://cloud-images.ubuntu.com/ - most notably LTS
releases, current stable release and the current development release.
