# CardinalOS
---------------
Instructions
------------
### Prerequisites
To get started with CardinalOS, you'll need to get familiar with [Repo](https://source.android.com/source/using-repo.html) and Version Control with [Git](https://source.android.com/source/version-control.html).

To set up build environment:
```
sudo apt update && sudo apt upgrade
git clone https://github.com/akhilnarang/scripts --depth 1
cd scripts
bash setup/android_build_env.sh
```

### Sync CardinalOS source
```bash
repo init -u https://github.com/CardinalOS/manifest.git -b U
repo sync --current-branch --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j$(nproc --all)
```

### Build
```bash
. build/envsetup.sh
lunch cardinal_<DEVICE>-userdebug
mka cardinal
```

## Credits:
* [AOSP](https://android.googlesource.com)
* [ArrowOS](https://github.com/ArrowOS)
* [DerpFest](https://github.com/DerpFest-AOSP)
* [DotOS](https://github.com/DotOS)
* [LineageOS](https://github.com/LineageOS)
* [PixelExperience](https://github.com/PixelExperience)
* [xdroidOS](https://github.com/xdroid-oss)
