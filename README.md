Pitch Black Recovery (UNOFFICIAL) for Samsung Galaxy a14x

| 📦 Device Info

    Device Codename: a14x
    Maintainer: PARBINDAR7

🛠 HOW TO BUILD

    Syncing OrangeFox Source (Branch 12.1)
    mkdir ~/OrangeFox_sync
    cd ~/OrangeFox_sync
    git clone https://gitlab.com/OrangeFox/sync.git
    cd ~/OrangeFox_sync/sync/
    ./orangefox_sync.sh --branch 12.1 --path ~/fox_12.1

🧭 Step 2: Navigate into the sync directory

    cd ~/fox_12.1

📂 Clone Device & Common Trees

    # Clone the device tree 
    git clone https://github.com/TeamWin/android_device_samsung_a14x.git device/samsung/a14x
 
    # Clone the common tree 
    git clone https://github.com/TeamWin/android_device_samsung_s5e8535-common.git device/samsung/s5e8535-common

⚙️ Step 4: Export Required Build Variable

    export ALLOW_MISSING_DEPENDENCIES=true

⚙️ Build

    # Set up build environment
    source build/envsetup.sh

    # Choose your device
    lunch twrp_a14x-eng

    # Start the build
    mka recoveryimage

⚠️ Disclaimer

This is an unofficial build. If you encounter any issues or features in the recovery that do not work as expected, please be aware that troubleshooting and fixes are your own responsibility.
If the recovery does not boot, gets stuck at the boot logo, or if you encounter issues related to the recovery image size being too large, please refer to the official troubleshooting guide - https://wiki.orangefox.tech/dev/building for detailed instructions to resolve these problems.
