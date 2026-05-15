# Changelog

The **Next** series continues development of the plugin by the original author and focuses on ongoing maintenance, reliability improvements, and compatibility with current Unraid releases.

Development of the plugin will continue with ongoing fixes, enhancements, and maintenance improvements.

## 2026.05.15

### Fixes
- Disk shares incorrectly added to Recycle Bin and share size calculations broken when they are added.

## 2026.05.10

### Fixes
- Fixes to recycle-delete to work on the CWD and trigger inotify for File Activity and Recycle Bin.

## 2026.05.03

### Fixes
- Boot up generating an error and double start of the recycle bin.

### Enhancements
- Add command 'recycle-delete' to delete files to a Recycle Bin share from the command line

## 2026.03.27

Initial release of the **Next** series maintained by the original author.

The focus of this release is reliability, stability, and improved operational behavior...

Several issues reported by users in previous versions have been addressed, including improvements to inotify monitoring, recycle bin logging, trash size calculations, and share handling.

Additional work has been done to reduce unnecessary Samba restarts, improve compatibility with recent Unraid UI changes, and enhance diagnostics to make troubleshooting easier.

### Major Improvements
- Significant reliability improvements to recycle bin handling and monitoring
- Refactored inotify event processing and logging for improved stability
- Improved trash size calculations and performance
- Reduced unnecessary service restarts to minimize Samba disruptions
- Improved compatibility with Unraid 7.x responsive UI changes

### Fixes
- Resolved multiple issues affecting recycle bin operation across shares
- Corrected inotify startup, shutdown, and error handling behavior
- Fixed several UI layout and responsiveness issues
- Addressed problems with recycle bin operation on special shares and devices
- Corrected several edge cases that could cause Samba instability

### Enhancements
- Added improved logging and diagnostics for troubleshooting
- Added recycle bin status indicators and monitoring improvements
- Added troubleshooting tools to help verify recycle bin operation
- Added smarter handling of Unassigned Devices shares
- Improved share detection and sorting behavior

### Operational Improvements
- Reduced logging noise and improved log clarity
- Limited inotify monitoring scope to `.Recycle.Bin` for better performance
- Improved configuration validation and safety checks

### Notes
- Minimum supported Unraid version is now **6.12**
- This release resumes active development of the plugin
- Detailed technical changes are documented in the GitHub release notes
