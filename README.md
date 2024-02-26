OrionOS
===========

Getting started
---------------

To get started with Android/OrionOS, you'll need to get familiar with [Source Control Tools](https://source.android.com/setup/develop).

To initialize your local repository using the LineageOS trees, use a command like this:
```
repo init --depth=1 -u https://github.com/OrionOS-Project/manifests.git -b 13 --git-lfs
```
Then to sync up:
```
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
To build, use following the commands:
```
. build/envsetup.sh
orion_$device-userdebug
m orion -j$(nproc --all)
```

