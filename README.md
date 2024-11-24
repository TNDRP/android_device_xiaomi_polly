# Android device tree for Xiaomi poco x6 (polly)

# How-to compile it:

- twrp-12.1 Manifest
```
    repo init --depth=1 -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp.git -b twrp-12.1
```
 - Sync
```
    repo sync
```
 - Clone TheNoobDevs-Staging twrp tree
```
    git clone https://github.com/TNDRP/android_device_xiaomi_polly.git -b android-14 device/xiaomi/polly
```
 - Build
```
    export ALLOW_MISSING_DEPENDENCIES=true; . build/envsetup.sh; lunch twrp_polly-eng; mka recoveryimage
```
