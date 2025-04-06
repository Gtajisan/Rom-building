# Custom ROM Building Tutorial

## Developer
Made by **Farhan**  
Made in **Bangladesh**

## Get Help
For build help and discussions, you can join the following GitHub channels:
- [@farhan_build](https://github.com/farhan_build)
- [@Farhan_build_discussion](https://github.com/Farhan_build_discussion)

## YouTube Tutorials
To get a better understanding of the custom ROM building process, here are some helpful YouTube videos:
- [How to Build a Custom Android ROM from Scratch](https://www.youtube.com/watch?v=example1)
- [AOSP ROM Build Tutorial](https://www.youtube.com/watch?v=example2)
- [LineageOS Custom ROM Build Guide](https://www.youtube.com/watch?v=example3)

## Custom ROM GitHub Sources
Here are some popular custom ROM GitHub repositories for reference and learning:
- [LineageOS](https://github.com/LineageOS/android)  
  AOSP-based custom ROM with a focus on performance and stability.
  
- [Pixel Experience](https://github.com/PixelExperience)  
  A custom ROM that brings a stock Pixel experience to various devices.
  
- [Resurrection Remix](https://github.com/ResurrectionRemix)  
  A feature-packed custom ROM based on AOSP, offering customizations and features.
  
- [AOSP](https://android.googlesource.com/platform/manifest)  
  The official Android Open Source Project source code for building your own ROM.

- [CrDroid](https://github.com/crdroidandroid)  
  A custom ROM designed to increase performance and reliability while offering rich features.

- [Dirty Unicorns](https://github.com/DirtyUnicorns)  
  A ROM with a unique set of features and an emphasis on providing a customizable experience.

- [Havoc OS](https://github.com/Havoc-OS)  
  A custom ROM that offers a rich set of features while keeping things close to stock Android.

- [CarbonROM](https://github.com/CarbonROM)  
  A lightweight and feature-rich custom ROM based on AOSP.

- [AOKP](https://github.com/AOKP)  
  A custom ROM with a unique user interface and several enhancements over AOSP.

## Device Recommendations
Before you begin, ensure your device is supported. Here are some devices that are popular in the custom ROM community:

- **Google Pixel 5**  
  A highly recommended device with official support from many custom ROMs like LineageOS and Pixel Experience.

- **OnePlus 8 Pro**  
  Known for its great performance and developer support, it's widely used for custom ROM development.

- **Xiaomi Redmi Note 10**  
  This budget-friendly device has good community support and works well with custom ROMs.

- **Samsung Galaxy S21**  
  Although it's a flagship phone, the device has extensive support for custom ROMs like LineageOS and Resurrection Remix.

- **OnePlus 6T**  
  An older device but with extensive support from the custom ROM community, including LineageOS and AOSP.

- **Essential Phone**  
  A phone with good developer support and great for custom ROMs like AOSP.

## Build Environment Setup

### Requirements
To build a custom ROM, you’ll need the following tools and software:

- **Ubuntu 20.04 LTS (Recommended)**
  - Custom ROMs are best built on Linux, with Ubuntu being the most recommended distribution.
  - Ensure you have at least **16GB of RAM** and **100GB of free disk space** for building the ROM.

- **Java Development Kit (JDK)**
  - Install JDK 8 (preferred version) or newer. You can install it via:
    ```bash
    sudo apt update
    sudo apt install openjdk-8-jdk
    ```

- **Repo Tool**
  - The `repo` tool is used to manage multiple Git repositories. Install it via:
    ```bash
    sudo apt install repo
    ```

- **Android SDK & NDK**
  - You'll need Android SDK and NDK for building AOSP or custom ROMs. You can download them from the [Android developer website](https://developer.android.com/studio).

- **Build Dependencies**
  - Install the required build dependencies by running:
    ```bash
    sudo apt-get install bc bison build-essential ccache clang curl flex g++-multilib git lib64stdc++6 libncurses5-dev libsdl1.2-dev libssl-dev libwxgtk3.0-gtk3-dev lzop pngcrush rsync schedtool squashfs-tools xsltproc zip zlib1g-dev
    ```

### Setting Up the Build Environment

1. **Set Up Your Directory**
   Create a directory where you will store all ROM source files:
   ```bash
   mkdir ~/android/roms
   cd ~/android/roms

**Install dependencies**
``
sudo apt install openjdk-8-jdk git bc bison build-essential
``
**Sync the source code**
``
repo init -u https://android.googlesource.com/platform/manifest
repo sync -j4
``
**Set up the build environment**

source build/envsetup.sh
lunch aosp_device-userdebug

**Build the ROM**
``
make -j4
``
Troubleshooting
"Device not found" error: Ensure device trees are properly configured.

"Dependency errors": Install all necessary dependencies.

"Out of memory": Increase swap file size or use more RAM.

License
This ROM is licensed under the MIT License.


### Notes:
- **YouTube Video Links**: I've added placeholder links for YouTube tutorials. You can replace these with actual URLs to relevant videos that you find helpful or have created.
  
- **Images**: I've used placeholder images for steps like cloning the repository, installing dependencies, syncing the source, setting up the environment, and building the ROM. You can replace these with real screenshots or images that illustrate each step of the process. If you want, I can generate or edit images based on your actual content.
- 