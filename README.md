# Utils
Some basic utilities I've created.

## wsl-xdg-open
A drop-in replacement for `xdg-open` in a WSL environment, requiring zero
configuration (other than `explorer.exe` being in the PATH, which *should*
happen automatically). Install with `sudo ln -s wsl-xdg-open
/usr/local/bin/xdg-open`. Opens properly formatted URLs (ie.
`https://google.com` works, but `google.com` doesn't.), and existing
files/folders (both those found in WSL and those in Windows).

## changes
Print the name of all repos with changes in your current directory, and show
the results of `git status -s` for that folder. Using the `-s` or `--short`
flags will show only the names of the unclean repos, and `q` or `--quiet` will
silence any diagnostic messages we may normally print.
