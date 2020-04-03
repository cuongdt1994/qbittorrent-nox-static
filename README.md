# qbittorrent-nox-static

This repo contains a build script for `qbittorent-nox` to create a fully static automatically using the current releases of the main dependencies, and an install script for installing `qbittorent-nox` to your seedbox.

## Installation

This script can install my pre-built static qbittorrent-nox to your seedbox. Currently this script only supports seedbox with root privilege.  
This script has been tested on Debian 9/10, Ubuntu 16.04/18.04, CentOS 7/8, Fedora 31, Arch Linux, OpenSUSE. Slackware, AlpineLinux and Gentoo are not supported due to lack of systemd.  
Shared seedboxes without root privilege will be supported later. Running script with root privilege will install qbittorrent to `/usr/bin/qbittorrent-nox`, while without root it will be installed to `$HOME/.local/bin/qbittorrent-nox`.  
This script will also setup configuration, including systemd service and WebUI password.  

```shell
bash <(wget -qO- --no-check-certificate https://github.com/Aniverse/qbittorrent-nox-static/raw/master/install.sh) \
USERNAME PASSWORD
```
```shell
bash <(curl -Ls https://github.com/Aniverse/qbittorrent-nox-static/raw/master/install.sh) USERNAME PASSWORD
```

## Download

My qBittorrent static builds can be downloaded [here](https://sourceforge.net/projects/inexistence/files/qbittorrent/).  
Currently I only have built qBittorrent 4.2.1 with libtorrent 1.1.14, I'll add more versions soon.  

*qBittorrent was built with the following details:*

```
OS: Debian 10 (buster)
Arch: amd64 (x86_64)
Qt: 5.14.1
Libtorrent: 1.1.4.0
Boost: 1.72.0
OpenSSL: 1.1.1d
zlib: 1.2.11
```

## Credits

https://github.com/userdocs/qbittorrent-nox-static

https://gist.github.com/notsure2/f8eac873eb7298d89d551047779d8361
