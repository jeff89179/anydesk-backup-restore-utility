# anydesk-backup-restore-utility
Simple macOS command file for backing up and restoring AnyDesk configuration.

This .command file opens in Terminal and will warn the user that it's about to close AnyDesk before continuing.
It will then present the user with the option Backup, Restore or Exit.

OPTIONS
1. Backup will change directories to the current user's home directory, zip the contents of .anydesk and save the zip file to the user's desktop with the current date in YYYYMMDD format.
2. Restore will bring up a file selection dialog in Finder to allow the user to browse for the file to restore. It will then extract it to the user's home folder. 
0. Exits

Once you open AnyDesk after restoring the backed up config, it should have all of the previously saved connections and histories.

NOTE: THIS IS STILL A WORK IN PROGRESS. Currently, it pulls in the .anydesk/incoming folder - which can contain some larger files from the File Transfer function of AnyDesk. I will eventually figure out how to exclude this in a future version.
