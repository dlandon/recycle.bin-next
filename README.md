# Recycle Bin - Next
Original author and continued development: Dan Landon

Recycle Bin - Next provides enhanced SMB safe-delete functionality for Unraid, including restore support, automated cleanup, detailed logging, and powerful log filtering to quickly locate deleted files.

The Recycle Bin Deleted and Removed log viewers support filtering by multiple search terms, wildcard matching (* and ?), and exclusion filters using !, making it easy to isolate the events you're looking for.

## Known Limitations (Read First)

Recycle Bin operates only on deletes performed over SMB/CIFS.

Deletes from the Unraid web UI, command line, Docker containers, or virtual machines bypass the recycle bin by design.

Recycle Bin does not operate on root shares (`/mnt/user` or `\\tower\`). Root shares are not actual Samba shares. Only individual user shares are supported.

The recycle bin relies on Samba's VFS recycle mechanism. This is a Samba limitation.

If a delete did not occur over SMB on an individual share, it will not be recycled.

## Features

- Per-share `.Recycle.Bin` folders with restore support.
- Automatic cleanup of recycled files based on age.
- Deleted Files log for auditing recycle activity.
- Flexible log filtering with multiple search terms, wildcard matching (`*` and `?`), and exclusion filters using `!`.
- Compatible with Custom SMB Shares while storing recycled files in the parent Unraid share's recycle bin.

## About This Project

The Next series of this plugin is actively maintained by the original author and continues development of the project with ongoing fixes, improvements, and enhancements.

## About This Project

The Next series of this plugin is actively maintained by the original author and continues development of the project with ongoing fixes, improvements, and enhancements.

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

For support, feature requests, and discussions, please use the Discussions tab.

## Distribution

This repository is the official distribution location for this plugin.

Users should install the plugin directly from the URLs provided in this repository to ensure they receive authentic and up-to-date releases.

Redistribution of this software through third-party repositories, plugin catalogs, mirrors, or repackaged installers is not authorized unless explicitly approved in writing by the author.

## License

This repository is maintained by the original author of the plugin.

Versions of this software publicly released prior to **March 18, 2025** remain licensed under the GNU General Public License (GPL) in accordance with their original terms.

Versions released as Next after that date are governed by the plugin-specific license included in the `LICENSE.md` file in this repository.

Users may install and use this software in accordance with the terms of that license.

## Support Development

If this plugin has been useful to you and you'd like to support ongoing development, you can optionally make a donation:

[Donate via PayPal](https://www.paypal.com/us/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=EJGPC7B5CS66E)

Feedback, bug reports, and success stories are also appreciated and help guide future development.

Support is appreciated, but never expected.
