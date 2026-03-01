# Recycle Bin – Next

Recycle Bin (Next) provides enhanced SMB safe-delete functionality for Unraid, including undo support, automated cleanup, and detailed logging.

### Known Limitations (Read First)

Recycle Bin operates only on deletes performed over SMB/CIFS.

Deletes from the Unraid web UI, command line, Docker containers, or virtual machines bypass the recycle bin by design.

Recycle Bin does not operate on root shares (/mnt/user or \\tower\).
Root shares are not actual Samba shares. Only individual user shares are supported.

The recycle bin relies on Samba’s VFS recycle mechanism.
This is a Samba limitation.

If a delete did not occur over SMB on an individual share, it will not be recycled.

### About This Project

This project continues development of the Recycle Bin plugin originally authored by Dan Landon, with enhancements, stability improvements, and expanded logging.

Development in this repository reflects ongoing work by the original author.

All versions publicly released under the GPL prior to March 6, 2025 remain licensed under the GPL.
Versions released after that date are governed by the custom license included in this repository.

For support, discussions, and announcements, please use the Discussions tab.

### Installing Recycle Bin (Next)

To install manually, enter one of the URLs below in the “Enter URL” field on the Unraid Plugins page.

Latest version:
https://raw.githubusercontent.com/dlandon/recycle.bin-next/master/recycle.bin-next.plg

Specific version:
https://raw.githubusercontent.com/dlandon/recycle.bin-next/vYYYY.MM.DD/recycle.bin-next.plg

Replace YYYY.MM.DD with the release date of the version you wish to install.
Include the leading v in the URL.

### License Notice

This repository is maintained by the original author of the Recycle Bin plugin.

Individual users may install and use this software in accordance with the license terms.

Versions released prior to March 6, 2025 remain licensed under the GPL.
Subsequent versions are licensed under the custom license included in this repository.
