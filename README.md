Build for Xiaomi Mi Mix 2

[Android Open Kang Project](http://aokp.co)
====================================

![Kanged Unicorn](http://aokp.co/images/cms-images/106.png)

Download the Source
===================

Please read the [AOSP building instructions](http://source.android.com/source/index.html) before proceeding.

Initializing Repository
-----------------------

To build: repo init -u https://github.com/hondajohn88/Build_Xiaomi_ROMs -b aokp-chiron-oreo

Additional required files to build this rom include:

Snapdragon LLVM compiler: snapdragon-llvm-4.0.2-linux64
Linaro Toolchain 5.5: gcc-linaro-5.5.0-2017.10-x86_64_aarch64-linux-gnu
Place snapdragon llvm compiler in /prebuilts Place linaro toolchain 5.5 in prebuilts/gcc/linux-x86/aarch64 and rename folder to gcc-linaro-5.5.0

Make sure you have qcom/common with sdllvm-lto-defs.mk in it.

Sync the repository:

    $ repo sync --force-sync

***

Building
--------

After the sync is finished, please read the [instructions from the Android site](http://s.android.com/source/building.html) on how to build.

    . build/envsetup.sh
    lunch

You can also build for specific devices (eg. chiron) like this:

    . build/envsetup.sh
    lunch aokp_chiron-userdebug
    mka rainbowfarts

Remember to `make clobber && make clean` every now and then!
