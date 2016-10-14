### Linux Intel DRM Nightly Branch

For my Dell XPS 13 9350, I feel as though Intel is bringing quite a few patches for stability/performance/powersaving.  
Instead of waiting for them to be merged to Mainline, why not just use the Intel DRM branch?

### Branches

* master - direct clone from https://cgit.freedesktop.org/drm-intel/log/?h=drm-intel-nightly without any patches
* nvme - NVME power saving patches
* drm-intel-testing - Testing instead of nightlies 

### Patches

Included patches:

NVME powersaving patches
BFQ patch
CK patch
GCC optimization

I'll include links later.

### Recommended Install
git clone https://github.com/victortrac/Intel-DRM-Nightly
git checkout <BRANCH>

makepkg -s

sudo pacman -U linux-*-`date +%Y%m%d`-1-x86_64.pkg.tar.xz 

Note: Please use proper package names for above.
