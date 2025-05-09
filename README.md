# INCDU
IFX thin wrapper script over NCDU to exclude custom directories.
Helps save precious time when you got to clear your local user directory in unix.

I wanted to inform you, this was rolled out as a small tool in Villach, which might help users find files/folders with large space consumption.
As of now, only available in VIH. We will roll that out to all RD sites, during their dedicated service dates.
Please don't start it on very large directories like /opt/tmp_share, that would take days to complete. ;)

This is available on all Compute and Login Hosts.

incdu (wrapper for ncdu)
ncdu is a graphical console alternative to du.
It provides a fast way to see which directories are using much space.
You can even browse the directories and erase files/dirs with it.

Since we got the ".snapshot" directory on every nfs share, we've provided a wrapper.
"incdu" will just ignore the snapshot directories.


 incdu - lists space usage in the current directory

 incdu <path> - lists space usage for a specific directory

<button style="background-color: orange; color: white; padding: 10px; border-radius: 25px;">Styled Button</button>

Up, down, j, k Cycle through the items
right, enter, l Open selected directory
s Order by filesize (press again for descending order)
d Delete the selected file or directory. An error message will be shown when the contents of the directory do not match or do not exist anymore on the filesystem
r Refresh/recalculate the current directory.
