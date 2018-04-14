# Build-Mi Mix 2
Manifest for Xiaomi MI Mix 2

To build: repo init -u https://github.com/hondajohn88/Build_Xiaomi_ROMs -b carbon-chiron-oreo

Additional required files to build this rom include:
 - Snapdragon LLVM compiler: snapdragon-llvm-4.0.2-linux64
 - Linaro Toolchain 5.5: gcc-linaro-5.5.0-2017.10-x86_64_aarch64-linux-gnu
 
 Place snapdragon llvm compiler in /prebuilts
 Place linaro toolchain 5.5 in prebuilts/gcc/linux-x86/aarch64
 
 Make sure you have qcom/common with sdllvm-lto-defs.mk in it.
