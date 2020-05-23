# About

Sink is a very simple backup tool. It relies on symbolic links to track
files and directories on you system. Then it uses rsync to save
backup copies of them to a destination directory. Rsync has the benifit
of detecting if a file has already been backed up or has been modified.
In these cases, rsynce only needs to transfer the difference between the
actual and the backed up copy. Sink is likely most useful when your backup
will reside on network attached storage or an external hard drive.


# Usage

Make a directory on you backup destination.
* `mkdir /Volumes/user/auto-backups`

Create a link to that directory.
* `./backup-to /Volumes/user/auto-backups`

You can place files the tracking directory.
* `mv ~/Downloads/bookmarks.html tracking`

Or create a link in tracking to a file or directory.
* `./start-tracking ~/Documents`

Then backup the data being tracked to its destination.
* `./sink`

You can also check logs from the backup process.
* `less history.log`


## Tips

* The backup destination must be present when you sink.

* You should only use absolute paths with this tool.

* You probably shouldn't track any directory that contains this tool.


## Scheduling

You could schedule this as a recurring job with cron.

A simplier way to automate backups might be to run sink at login with .profile.

Better yet, you could run sink 20 minutes after login.
This gives time for startup processes to finish and
for connecting to network storage.

* `sinklater() { sleep 1200; ~/repos/sink/sink; } sinklater &`
