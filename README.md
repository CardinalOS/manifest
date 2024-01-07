# CardinalOS

Getting Started:
==============

To get started with CardinalOS, you'll need to get familiar with [Repo](https://source.android.com/source/using-repo.html) and Version Control with [Git](https://source.android.com/source/version-control.html).

To initialize your local repository, use a command like this:
```bash
repo init -u https://github.com/CardinalOS/manifest.git -b udc
```

You can alternatively use this command to save some space and time :
```bash
repo init --depth=1 -u https://github.com/CardinalOS/manifest.git -b udc
```

Then to sync up:
```bash
repo sync --current-branch --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j$(nproc --all)
```
---------------------------------------------------------------------------------------
Compilation:
==================
```bash
. build/envsetup.sh
lunch cardinal_<DEVICE>-userdebug
mka cardinal
```
---------------------------------------------------------------------------------------
Credits:
=======
* [AOSP](https://android.googlesource.com/)
* [LineageOS](https://github.com/LineageOS)
* [PixelOS](https://github.com/PixelOS-Fourteen)
* [xdroidOS](https://github.com/xdroid-oss)
* [**ManyMore from where cherry-picked from**](https://github.com)
---------------------------------------------------------------------------------------
