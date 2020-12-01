# Introduction

This project would be an upgrade to the [Paragon NTFS driver for Linux](https://www.paragon-software.com/home/ntfs-linux-professional/).

That driver comes with a [Free Limited Version](https://www.paragon-software.com/home/ntfs-linux-professional/#comparison) which can be downloaded by [this official link](http://dl.paragon-software.com/free/Paragon-715-FRE_NTFS_Linux_9.5_Express.tar.gz).

## License

In order to publish this project, antonio-petricca received the written (Email) permission from Paragon which asked him to publish:

- [Paragon - End User License](https://raw.githubusercontent.com/luhuachuixue/ufsd/main/Paragon-End-User-License.txt)
- [Paragon - General terms and conditions](https://raw.githubusercontent.com/luhuachuixue/ufsd/main/Paragon-General-terms-and-conditions.pdf)
- [Paragon - Data protection policy](https://raw.githubusercontent.com/luhuachuixue/ufsd/main/Paragon-Data-protection-policy.pdf)

## State of the art

At the time antonio-petricca was writing (September 26, 2018) it supports kernel up to the 4.12.

## Goals

The goal of this project is to support kernels 4.13 and newers.

## How to build

The `apply-patches` script downloads the [free limited version](http://dl.paragon-software.com/free/Paragon-715-FRE_NTFS_Linux_9.5_Express.tar.gz) of the driver, then patches it to work on newer kernel releases.

```bash
./apply-patches
cd sources
./configure
make driver
sudo make driver_install
```