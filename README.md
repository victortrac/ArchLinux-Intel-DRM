### Archlinux Linux Intel DRM Kernels
These are Archlinux custom kernels built from upstream DRM Intel kernel patches.

I use these to make my Dell XPS 13 9350 run a little better, specifically with getting USB-C to handle 4k @ 60Hz external displays.

### Branches

* drm-intel-nightly
* drm-intel-nightly-9350 - This is a stripped down kernel customized for the XPS 9350. May not support all your peripherials!
* drm-intel-testing 
* nvme - NVME power saving patches

### Recommended Install

    git clone https://github.com/victortrac/ArchLinux-Intel-DRM
    git checkout <BRANCH>
    makepkg -s
    sudo pacman -U linux-*-`date +%Y%m%d`-1-x86_64.pkg.tar.xz 
