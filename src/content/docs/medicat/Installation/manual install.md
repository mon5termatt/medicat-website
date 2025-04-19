---
draft: false
title: "Manual Installation Guide"
publishDate: "2024-4-19"
category: "Installation"
author: "MON5TERMATT"
tags: [medicat, installation, manual, guide]
---

# Manual Installation Guide

## ⚠️ Important Pre-Installation Steps

1. **Disable Antivirus**
   - Open your Antivirus software
   - Disable Real-Time protection
   - Temporarily disable any other security features that might interfere with the installation

2. **Download Required Software**
   - [Ventoy](https://www.ventoy.net/en/download.html) - Bootable USB creator
   - [7-Zip](https://www.7-zip.org/download.html) - For extracting .7z files
   - [Medicat](https://medicatusb.com#downloads) - Latest release

## Installation Steps

### 1. Prepare Your USB Drive
- Insert your USB drive (minimum 32GB recommended)
- Backup any important data from the USB drive as it will be formatted
- Open Windows Disk Management to verify the drive letter

### 2. Install Ventoy
1. Download and extract Ventoy
2. Run `Ventoy2Disk.exe` as Administrator
3. Select your USB drive from the dropdown menu
4. Click "Install" and wait for the process to complete
5. Verify the installation was successful

### 3. Format the USB Drive
1. Open Windows File Explorer
2. Right-click on your USB drive
3. Select "Format"
4. Choose the following settings:
   - File System: NTFS
   - Allocation Unit Size: Default
   - Quick Format: Checked
5. Click "Start" and wait for formatting to complete

### 4. Extract Medicat
1. Download the latest Medicat .7z file
2. Right-click the .7z file and select "7-Zip" > "Extract Here"
3. Copy all extracted files to the root of your USB drive
4. Verify the following folders and files are present:
   ```
   USB_DRIVE/
   ├── Antivirus/
   ├── Backup/
   ├── Backup_and_Recovery/
   ├── Boot_Repair/
   ├── Diagnostic_Tools/
   ├── Live_Operating_Systems/
   ├── OSimages/
   ├── Partition_Tools/
   ├── Password_Removal/
   ├── PortableApps/
   ├── Programs/
   ├── System/
   ├── ventoy/
   ├── VHD/
   └── Windows_Recovery/
   ```

### 5. Final Verification
1. Ensure all directories and files listed above are present
2. Verify that `Start.exe` is present in the root directory
3. Check that the `ventoy` directory contains the necessary boot files
4. Safely eject your USB drive

## Post-Installation

1. Re-enable your Antivirus software
2. Test the USB drive by booting from it
3. If you encounter any issues, refer to the [Troubleshooting Guide](/docs/medicat/support/troubleshooting/)

## Alternative Installation Method

If you prefer an automated installation process, you can use the [Windows Auto Installer](https://github.com/mon5termatt/medicat_installer/releases) which handles all these steps automatically.
