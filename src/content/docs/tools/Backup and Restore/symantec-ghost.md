---
title: Symantec Ghost
description: Documentation for Symantec Ghost in MediCat USB
---

# Symantec Ghost

Symantec Ghost (Ghost Solution Suite) is a powerful disk cloning and imaging solution.

## Overview

Symantec Ghost, which stands for "General Hardware-Oriented System Transfer," is a disk cloning tool used primarily for disk cloning, disk imaging, and deploying Windows operating systems to multiple computers. It's widely used in enterprise environments for system deployment and backup.

## Key Features

- **Disk Cloning**: Create exact copies of disks for migration or deployment
- **Disk Imaging**: Create and restore disk images for backup and recovery
- **Multicast Deployment**: Deploy images to multiple computers simultaneously
- **Hardware-Independent Restoration**: Deploy images to different hardware configurations
- **Boot Disk Creation**: Create bootable recovery media
- **Scripting Support**: Automate deployment and recovery tasks

## Usage in MediCat

In MediCat USB, Symantec Ghost can be used to:

1. Create system backups
2. Clone disks for hardware upgrades
3. Deploy standard system configurations to multiple computers
4. Restore systems after failures

## Getting Started

1. Boot from the MediCat USB drive
2. Navigate to the Backup and Recovery section
3. Select Symantec Ghost
4. Choose between creating an image, restoring an image, or cloning a disk

## Common Commands

- **Ghost32.exe -clone,mode=create,src=1,dst=c:\image.gho**: Create an image of the first disk
- **Ghost32.exe -clone,mode=restore,src=c:\image.gho,dst=1**: Restore an image to the first disk
- **Ghost32.exe -clone,mode=copy,src=1,dst=2**: Clone disk 1 to disk 2

---

*Disclaimer: This documentation was generated with AI assistance and may require review for complete accuracy and up-to-date information.*
