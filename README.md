# TWRP device tree for Samsung Galaxy Tab A 8.0 LTE (2019)

> ## DISCLAIMER
>
> This device tree is not an official device tree and is not in any way
> endorsed by, sponsored by, or affiliated with the Team Win Recovery team
> and/or project.

## SM-P205

Add to `.repo/local_manifests/wisdom.xml`:
```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="sethmurphy18/android_device_samsung_wisdom" path="device/samsung/wisdom" remote="github" revision="android-9.0" />
</manifest>
```
Then run `repo sync` to check it out.

___

To build:
```
. build/envsetup.sh
lunch omni_wisdomub-eng
make recoveryimage
```

___

Kernel source: [Samsung Open Source](https://opensource.samsung.com/uploadSearch?searchValue=SM-P205)

## Maintainer Notes

You may notice a lot of similarities bewtween this repository and the
repository for the [SM-T515](https://github.com/Magendanz/android_device_samsung_gta3xl),
that's no coincidence. The GTA3XL and WISDOM are basically the same device,
with a different size screen. They even have the same resolution, so I
started with that device repository as a starting point, then built from there.