---
draft: false
title: "Medicat Installer"
publishDate: "2025-4-19"
category: "Install"
author: "MON5TERMATT"
tags: [medicat, install, installer]
---

# Medicat Installer

[View the Main Installer Repo](https://github.com/mon5termatt/medicat_installer)

## Installation Methods

### Windows Installation
1. Download the Windows installer script from the repository
2. Right-click the script and select "Run as Administrator"
3. Follow the on-screen prompts to complete the installation
4. The installer will automatically:
   - Format your USB drive
   - Copy all necessary files
   - Set up the boot configuration
   - Create the required partitions

### Linux Installation
1. Download the Linux installer script
2. Open a terminal in the script's directory
3. Make the script executable:
   ```bash
   chmod +x medicat_installer.sh
   ```
4. Run the script with sudo privileges:
   ```bash
   sudo ./medicat_installer.sh
   ```
5. Follow the interactive prompts to complete the installation

## Notes
- The installer requires administrative privileges
- Installation time varies based on your USB drive speed
- A minimum of 32GB USB drive is recommended
- Always backup your data before proceeding with installation
