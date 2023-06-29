<img src="https://github.com/PixelOS-AOSP/official_devices/blob/thirteen/banners/latest.png?raw=true">

# PixelOS

 Getting Started
---------------
To get started with the PixelOS sources, you'll need to get
familiar with [Git and Repo](https://source.android.com/setup/build/downloading).

 To initialize your local repository, use command:

```bash
repo init -u https://github.com/pos-gm/manifest.git -b thirteen
```

```bash
repo init --depth=1 -u https://github.com/pos-gm/manifest.git -b thirteen
```

Then sync up:

```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

Building the System
-------------------
 Initialize the ROM environment with the envsetup.sh script.

```bash
. build/envsetup.sh
```

Lunch your device after cloning all device sources if needed.

```bash
lunch aosp_devicecodename-buildtype
```

Start compilation

```bash
make bacon
```
