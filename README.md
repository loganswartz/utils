# Utils
Some basic utilities I've created.

## wsl-xdg-open
A drop-in replacement for `xdg-open` in a WSL environment, requiring zero
configuration (other than `explorer.exe` being in the PATH, which *should*
happen automatically). Install with `sudo ln -s wsl-xdg-open
/usr/local/bin/xdg-open`. Opens properly formatted URLs (ie.
`https://google.com` works, but `google.com` doesn't.), and existing
files/folders (both those found in WSL and those in Windows).
