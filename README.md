# Recycle Bin - Next
Original author and continued development: Dan Landon

Recycle Bin - Next provides enhanced SMB safe-delete functionality for Unraid, including undo support, automated cleanup, and detailed logging.

## Known Limitations (Read First)

Recycle Bin operates only on deletes performed over SMB/CIFS.

Deletes from the Unraid web UI, command line, Docker containers, or virtual machines bypass the recycle bin by design.

Recycle Bin does not operate on root shares (`/mnt/user` or `\\tower\`). Root shares are not actual Samba shares. Only individual user shares are supported.

The recycle bin relies on Samba’s VFS recycle mechanism. This is a Samba limitation.

If a delete did not occur over SMB on an individual share, it will not be recycled.

## About This Project

This repository contains the continued development of the Recycle Bin plugin originally authored by Dan Landon.

Development in this repository is maintained by the original author and includes enhancements, stability improvements, and expanded logging.

Versions of this software publicly released prior to **March 18, 2025** were licensed under the GNU General Public License (GPL) and remain licensed under the GPL in accordance with their original terms.

Versions released after that date are governed by the **Recycle Bin - Next Personal Use License v1.0** included in this repository.

## Installing Recycle Bin - Next

To install manually, enter one of the URLs below in the **Enter URL** field on the Unraid Plugins page.

### Latest version

Copy the URL exactly as shown:
https://raw.githubusercontent.com/dlandon/recycle.bin-next/master/recycle.bin-next.plg

### Specific version

Copy the URL exactly as shown:
https://raw.githubusercontent.com/dlandon/recycle.bin-next/vYYYY.MM.DD/recycle.bin-next.plg

Replace `YYYY.MM.DD` with the release date of the version you wish to install. Include the leading `v` in the URL.

**Note:** The URL must begin with `https://raw.githubusercontent.com/`. GitHub page URLs (`github.com/.../blob/...`) will not install correctly.

## Distribution

This repository is the official distribution location for this plugin.

Users should install the plugin directly from the URLs provided in this repository to ensure they receive authentic and up-to-date releases.

Redistribution of this software through third-party repositories, plugin catalogs, mirrors, or repackaged installers is not authorized unless explicitly approved by the author.

## License

This repository is maintained by the original author of the plugin.

Versions of this software publicly released prior to **March 18, 2025** remain licensed under the GNU General Public License (GPL) in accordance with their original terms.

Versions released after that date are governed by the plugin-specific license included in the `LICENSE.md` file in this repository.

Users may install and use this software in accordance with the terms of that license.
