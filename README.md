## TWRP device tree for Galaxy Note 4 (China Duos)

Add to `.repo/local_manifests/trltezc.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/samsung/trltezc" name="android_device_samsung_trltezc" remote="TeamWin" revision="android-6.0" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_trltezc-eng
make -j5 recoveryimage
```

Kernel sources are available at: https://github.com/jcadduono/nethunter_kernel_trlte/tree/twrp-5.1

