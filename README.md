Prerequisites
------
- `bash`, `curl`, `grep`, `coreutils`, `jq`
- media player, capable of playing http streams (`vlc`, `mpv`)
- living in 🇧🇬

Installation
---------
Use your distribution way of packaging. You can just copy items in their respective paths, but **untracked** files are bad idea to put software.

Edit `/usr/bin/tv` to respect your choice of media player:
- VLC:
```
[[ -n $URL ]] && vlc --http-referrer=$R $URL &
# [[ -n $URL ]] && mpv --force-seekable --force-window --referrer=$R $URL &
```

License
-----------
GNU General Public License v3.0 or later (`GPL-3.0-or-later`)
