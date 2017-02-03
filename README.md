# syncunionfstorclone
This script syncs all deleted files and directories on your unionfs-fuse mount with your rclone destination. It also moves all files and directories of your unionfs-fuse read/write mount to your rclone destination.<br>

To run this script, you need to have rclone and unionfs-fuse already installed and configured.<br>

Place this script in your target directory and set:
```chmod a+x /path/to/script/syncunionfstorclone```

Change these parameters for you needs:
* UNIONFSRWPATH (your unionfs-fuse read/write directory)
* RCLONEDEST (your rclone Destination
* MINAGE (files and folder older this value will be deleted or moved on/to your rclone destionation)

You can run this script manually, or by cron. This example runs the script every minute:
```* * * * * /path/to/script/syncunionfstorclone```

Feel free to post questions or commencts in the issues section.
