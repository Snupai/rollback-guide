# :pushpin: Disclaimer
> I am not responsible for any damage, misuse or other kind of physical or mental damage which results in following this guide.
This repo is in no way shape or form affiliated with Nothing Technology Limited (NOTHING).

***

# :memo: Prerequisites:

### 1. Unlock Bootloader:

* Ensure that the bootloader on your device is unlocked. This is necessary for flashing custom images. Note that unlocking the bootloader may void your warranty and wipe your data. See Step 2 for instructions.

### 2. Install ADB and Fastboot:

* Download and install ADB and Fastboot on your computer. You can use the [Android SDK package](https://developer.android.com/tools/releases/platform-tools) or [15 Seconds Online ADB Installer and Updater](https://androidmtk.com/download-15-seconds-adb-installer).
> [!IMPORTANT]
> The installation of ADB and Fastboot must be system-wide (in PATH)

### 3. Download OS Image:

* Obtain the full OS image for your device. You can find the stock images on [reindex-ot](https://reindex-ot.github.io/). Scroll down to "Nothing Phone(1) Fastboot ROM (SourceForge)" and download the latest version.

***

# Steps to Boot the OS Image:

### 1. Enable Developer Options on your phone:

* Go to "Settings" > "About phone" > Tap "Build number" seven times to unlock Developer Options.

### 2. Enable OEM unlocking:

* In "Developer Options", enable "OEM unlocking". This unlocks the bootloader of your device

> [!IMPORTANT]
> Please lock the bootloader after the whole process has ended. (Note: this will wipe all data)

### 3. Enable USB Debugging:

* In "Developer Options," enable "USB Debugging." This allows your computer to communicate with your device.

### 4. Connect your Phone to your Computer:

* Use a USB cable to connect your phone to your computer. Make sure the connection is stable.

* Allow Debugging when prompted on your phone.

### 5. Open a Command Prompt or Terminal:

* Open a command prompt on Windows or a terminal on Linux/macOS.

### 6. Navigate to the ADB and Fastboot Directory:

* Use the `cd` command to navigate to the directory where ADB and Fastboot are installed.

```batch
cd path/to/adb/fastboot
```

### 7. Reboot into Fastboot Mode:

* Reboot your device into Fastboot mode. You can do this by executing the following command:

```batch
adb reboot bootloader
```
* Or by holding the volume down button and the power button until the device vibrates.

### 8. Verify Fastboot Connection:

* Ensure that your device is detected in Fastboot mode:

```batch 
fastboot devices
```

* If your device is listed, you're ready to proceed.

### 9. Install the OS Image:

* Install the OS image on your device. Simply run the Flash_slot_a.bat file.

### 10. Wait for the Device to Boot:

* When the Android Recovery Screen is shown choose `Factory data reset`. You can do so by pressing `vol +/-` to move in the list and `power button` to enter. On the next screen please confirm by choosing `Factory data reset`.
> [!NOTE]
> The first boot may take some time as the new OS is being set up. Be patient.

***

# Notes:

### Backup Data:

* Before flashing a new OS, it's advisable to back up important data on your device.

### Verify Compatibility:

* Ensure that the OS image you're booting is compatible with your device model.

### Community Resources:

* If you're using a custom ROM, refer to community forums or documentation for specific instructions.

***

* Remember that flashing custom ROMs or OS images carries risks, and you should be aware of the potential consequences. Always follow instructions provided by reliable sources and forums related to your specific device model.

If you find anything wrong with this guide feel free to correct me.
