---
draft: false
title: "Troubleshooting Guide"
publishDate: "2025-4-19"
category: "Support"
author: "MON5TERMATT"
tags: [medicat, troubleshooting, help, support]
---

# Troubleshooting Guide

## Common Installation Issues

### USB Drive Not Detected
- **Issue**: Ventoy or Windows doesn't recognize your USB drive
- **Solutions**:
  1. Try a different USB port (preferably USB 3.0 or higher)
  2. Check if the drive appears in Windows Disk Management
  3. Try a different USB drive
  4. Ensure the drive is properly formatted as NTFS

### Ventoy Installation Fails
- **Issue**: Error during Ventoy installation
- **Solutions**:
  1. Run Ventoy as Administrator
  2. Disable any antivirus software temporarily
  4. Use a different USB drive if the current one is problematic

### Extraction Errors
- **Issue**: Problems extracting the Medicat .7z file
- **Solutions**:
  1. Ensure you have the latest version of 7-Zip installed
  2. Verify the download is complete and not corrupted
  3. Verify the hash of the file
  4. Try extracting to a local drive first, then copy to USB
  5. Check if you have enough free space on your drive

## Boot Issues

### USB Won't Boot
- **Issue**: Computer doesn't boot from the USB drive
- **Solutions**:
  1. Enter BIOS/UEFI and ensure USB boot is enabled
  2. Try different USB ports
  3. Check if Secure Boot is disabled in BIOS
  4. Verify the boot order in BIOS settings

### Black Screen on Boot
- **Issue**: Screen goes black after selecting Medicat
- **Solutions**:
  1. Try booting in Legacy mode instead of UEFI
  2. Check if your graphics drivers are compatible
  3. Try different display ports or cables
  4. Wait a few minutes as some systems take longer to initialize

### Missing Tools or Features
- **Issue**: Certain tools or features don't appear
- **Solutions**:
  1. Verify all directories are present on the USB drive
  2. Check if the tool is included in your Medicat version
  3. Try recreating the USB drive
  4. Ensure you have enough free space on the USB drive

## Performance Issues

### Slow Loading Times
- **Issue**: Tools take too long to load
- **Solutions**:
  1. Use a USB 3.0 or higher drive
  2. Ensure your USB port supports USB 3.0 or higher
  3. Check if your system meets minimum requirements
  4. Try defragmenting the USB drive (if using HDD)

### Tool Crashes
- **Issue**: Specific tools crash or fail to run
- **Solutions**:
  1. Check if the tool requires additional dependencies
  2. Verify the tool is compatible with your system
  3. Try running the tool with administrator privileges
  4. Check the tool's documentation for specific requirements

## System Compatibility

### UEFI vs Legacy Boot
- **Issue**: Boot mode compatibility problems
- **Solutions**:
  1. Check your system's boot mode (UEFI or Legacy)
  2. Try both boot modes if available
  3. Update your system's firmware if possible
  4. Check if your system supports the required boot mode

### Hardware Compatibility
- **Issue**: Tools don't work with specific hardware
- **Solutions**:
  1. Check the tool's hardware requirements
  2. Update your system's drivers
  3. Try alternative tools with similar functionality
  4. Check if your hardware is supported by the tool

## Getting Additional Help

If you're still experiencing issues:
1. Check the [Medicat Discord](https://discord.gg/medicat) for community support
2. Review the [Installation Guide](/docs/medicat/Installation/) for detailed setup instructions

Remember to always backup your data before attempting any system repairs or modifications. 