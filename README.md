# PS3 Downgrade Guide

This guide will help you downgrade your PS3 to any very low firmware version. This can be great for re-selling a day one system.

## Steps

1. **Download Desired Firmware**
   - Download the `PS3UPDAT.PUP` file for the firmware version you want to downgrade to (e.g., 1.02).

2. **Download PUAD**
   - Download PUAD 1.2.

3. **Install PUAD**
   - Install PUAD 1.2 on your computer.

4. **Repack the PUP File**
   - Open PUAD.
   - Select the `Repacker` option.
   - Select the `PS3UPDAT.PUP` file for the desired firmware version.
   - In the image version field, type `99999` and highlight `manual`.
   - Select `UPL` in other options (it should be highlighted in blue).
   - Press `Start` and wait for the process to complete.

5. **Modify the XML File**
   - Go to `update_files/UPL.xml.pkg.decrypted`.
   - Select `content.xml` and open it with Notepad++.
   - Find the line that says `version` and change `01.02` (or the current version) to `99.99`.
   - Find the line that says `build` and change the original image build to `99999`.
   - Save the file.

6. **Repack the PUP File Again**
   - Go back to PUAD.
   - Select `Repack` and wait for the process to complete.
   - The new file should be saved as `NEW-PS3UPDAT.PUP`.

7. **Downgrade to 3.55 Rogero Downgrader**
   - Downgrade your PS3 to 3.55 Rogero Downgrader (this will not work with Rebug).

8. **Enable Toggle QA**
   - After downgrading to 3.55, enable `Toggle QA` from Rebug.

9. **Restart the System**
   - Restart your PS3 after enabling `Toggle QA`.

10. **Install Desired Firmware**
    - Put the `PS3UPDAT.PUP` for the desired firmware version on a USB stick in the `PS3/UPDATE` folder and rename it to `PS3UPDAT.PUP`.
    - Plug the USB stick into your PS3.
    - Install the desired firmware from the XMB (you do not need recovery mode for this).
    - Follow the installation screen instructions and let the firmware install.

11. **Alternative Version Handling**
    - If you encounter a "Data is corrupted" error during the installation, try using a different version like 1.90 and follow the same steps above to downgrade to the desired firmware.
    - Use MinVerChk to see what the lowest firmware for your console is.

## Additional Tips


- **Backup Your Data:** Before performing any downgrade or firmware changes, make sure to backup all important data from your PS3. Downgrading can potentially lead to data loss.
- **Ensure Power Stability:** Make sure your PS3 is connected to a stable power source during the entire process to prevent any interruptions that could harm your system.
- **Use Verified Sources:** When downloading PUAD or firmware files, use verified and trusted sources to avoid malware or corrupted files.

## Troubleshooting

- **Error: Data is Corrupted**
  - If you see this error during installation, it often means there's an issue with the PUP file. Double-check your steps in modifying the XML file and repacking the PUP file.
  - Try using a different firmware version (like 1.90) and follow the same steps to downgrade to the desired firmware.

- **Downgrade Not Starting**
  - Ensure that the `PS3UPDAT.PUP` file is correctly placed in the `PS3/UPDATE` folder on your USB stick.
  - Double-check that the USB stick is formatted to FAT32.

## Disclaimer

- **Risk of Bricking:** Downgrading your PS3 can be risky and may lead to potential issues, including bricking your device. Follow these instructions carefully and proceed at your own risk.
- **Warranty Void:** Performing a downgrade or any unofficial modifications to your PS3 will likely void any warranty you may have.

Hope this helps!
