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



- [![Up](https://img.shields.io/badge/UP-white)]() , [![Down](https://img.shields.io/badge/Down-white)]() ,[![J](https://img.shields.io/badge/J-white)]() ,[![K](https://img.shields.io/badge/K-white)]() Cycle through the items

- [![Right](https://img.shields.io/badge/Right-white)]() , [![Enter](https://img.shields.io/badge/Enter-white)]() , [![l](https://img.shields.io/badge/L-white)]() Open selected directory

- [![S](https://img.shields.io/badge/S-white)]()  Order by filesize (press again for descending order)

- [![D](https://img.shields.io/badge/D-white)]()  Delete the selected file or directory. An error message will be shown when the contents of the directory do not match or do not exist anymore on the filesystem

- [![R](https://img.shields.io/badge/R-white)]()  Refresh/recalculate the current directory.
