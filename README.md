# dis-wif-mag
Disable WiFi drivers via Magisk.

## Disclaimer and Important Notice
    DISCLAIMER 1: I assume no responsibility for any consequences arising from the use of this plugin. 
    Proceed with caution, as there is a risk of bricking your device.
    
    DISCLAIMER 2: It's important to note that ANYONE with access to Magisk can disable this plugin. 
    No protective measures have been implemented to prevent such actions. 
    Please be aware of this potential issue.

    To mitigate this risk, you may TRY to either concealing Magisk or implementing third-party password protection measures.

## Compatibility
Successfully Tested on:

    Samsung Tablet: Galaxy Tab A8
    Android Version: 13, OneUI Version: 5.1.1

## Usage Instructions
### Via User Interface (UI):

1. Download the latest release package.
2. Alternatively, download the repository and create a ZIP file.
3. Upload the package to your device.
4. Open Magisk.
5. Install the module from the ZIP file.
6. Reboot your device for the changes to take effect.

### Via ADB (Android Debug Bridge):
1. Execute the command: magisk --install-module /path/to/module.zip
2. Reboot your device to apply the changes.

# Creation and Functionality
Background:
* Explored files named wifi under /system and /vendor.
* Initially attempted patching driver XML files, but opted for a more "generic" approach to ensure compatibility with various devices.

Implementation:
* Generated dummy files (0 bytes) to replace WiFi drivers, allowing for a broad application across different devices.
