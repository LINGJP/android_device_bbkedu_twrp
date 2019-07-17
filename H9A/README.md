EEBBK S1 Pro
===============
```
By : LONEYQC
```
The S1 Pro (codename _"S1S"_) is a tablet from bbkedu.

This is a Minimal Device Tree for building TWRP for EEBBK S1 Pro (Codename: S1S). I used TWRP by multirom and TWRP for Asus Zenpad 3S 10 from rakomancha to finally build a working tree for S1 Pro.

Basic        | Spec Sheet
------------:|:------------------------
CPU          | Cortex-A72 & Cortex-A53 | Hexa-Core | MT8176
GPU          | PowerVR GX6250
Memory       | 4GB RAM
Shipped Android Version | 7.1
Storage      | 64GB
Battery      | 6600 mAh Li-Po
Display      | 7.9
Rear Camera  | 13.0 MP , Video
Front Camera | 5.0 MP


This branch is for building TWRP.

### Thanks to:
 * GEEK RomTeam
 * myself

### To build: 

```
$ mkdir twrp

$ cd twrp

$ repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-7.1

To initialize a shallow clone, which will save even more space, use a command like this:

$ repo init --depth=1 -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-7.1

After that sync your sources:

$ repo sync

Download or clone this repository, go to /twrp/device and create bbkedu/S1S. Copy this repo to your created folder

Build your recovery:

$ source build/envsetup.sh

& lunch S1S-eng

make clean && make recoveryimage
```
