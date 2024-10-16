# PixelOS

 Getting Started
---------------
To get started with the PixelOS sources, you'll need to get
familiar with [Git and Repo](https://source.android.com/setup/build/downloading).

 To initialize your local repository, use command:

```bash
repo init -u https://github.com/pixelos-gm.git -b fourteen --git-lfs
```

Then sync up:

```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
