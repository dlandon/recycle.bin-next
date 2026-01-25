# Recycle Bin - Next

Recycle Bin (Next) provides enhanced SMB safe-delete functionality for Unraid, including undo support, automated cleanup, and detailed logging.

**Recycle Bin - Known Limitations (Read First)**

Recycle Bin works only for deletes performed over SMB/CIFS.
Deletes from the Unraid web UI, command line, Docker containers, or VMs bypass the recycle bin by design.

Recycle Bin does not and cannot work on root shares (/mnt/user or \\tower\).
Root shares are not real Samba shares. Recycle Bin is only supported on individual user shares.

The recycle bin relies on Samba's VFS recycle mechanism.
This is a Samba limitation, not an Unraid-specific one.

If your delete did not occur over SMB on an individual share, it will not be recycled.

This plugin is an **independent alternative** to the official Unraid Recycle Bin plugin, offering bug fixes, enhanced safe-delete features, and logging.

This project continues the plugin authored by **dlandon** with enhancements and bug fixes.

Development in this repository begins from the codebase authored by **dlandon** and continues privately as of **March 2025**.

All development and commits dated **March 2025** and later are licensed under the custom license included in this repository.

For support, discussions, and announcements, please use the **Discussions** tab in this repository.

# Installing Recycle Bin

To install this plugin manually, enter either of the URLs below in the Enter URL field of the Plugins page.  The URL below will either install the latest or a specific version you choose.

Latest version: https://raw.githubusercontent.com/dlandon/recycle.bin-next/master/recycle.bin-next.plg

Specific version: https://raw.githubusercontent.com/dlandon/recycle.bin-next/vYYYY.MM.DD/recycle.bin-next.plg


Enter the release date "YYYY.MM.DD" of the specific version you want to install.  Be sure to keep the "v" before the release date.
### Notice

This repository is independently maintained by the original author of the Recycle Bin plugin.

Individual Unraid users may install and use this software in accordance with the license terms.

All versions of Recycle Bin released publicly under the GPL prior to March 2025 remain licensed under the GPL.

Limetech or other third parties may not incorporate this code into Unraid or other products without a separate licensing agreement.

