EEBBK MT8167 PLATFORM
===============
```
By : John-Romero
```
The EEBBK MT8167 PLATFORM (codename _"EMP"_) is a tablet from bbkedu.

This is a Minimal Device Tree for building TWRP for EEBBK MT8167 PLATFORM (Codename: EMP). I used TWRP by multirom and TWRP for Asus Zenpad 3S 10 from rakomancha to finally build a working tree for EMP.

Basic        | Spec Sheet
------------:|:------------------------
CPU          | Cortex-A53 | Hexa-Core | MT8167
GPU          | PowerVR GE8600
Memory       | 1/2GB RAM
Shipped Android Version | 7.0
Storage      | 16/32GB
Battery      | 6600 mAh Li-Po
Display      | 7.9
Rear Camera  | 8.0 MP , Video


This branch is for building TWRP.

### Thanks to:
 * Haozhe
 * LuoJingpei
 * John-Romero

### To build: 

```
$ mkdir twrp

$ cd twrp

$ repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-7.1

To initialize a shallow clone, which will save even more space, use a command like this:

$ repo init --depth=1 -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-7.1

After that sync your sources:

$ repo sync

Download or clone this repository, go to /twrp/device and create bbkedu/*. Copy this repo to your created folder

Build your recovery:

$ source build/envsetup.sh

& lunch *-eng

make clean && make recoveryimage
```
