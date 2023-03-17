# discord-linux-installer

Discord doesn't let users use outdated versions while also updating too sporadically, which makes it terrible for packaging in distros. So these scripts provide a way to install it manually to `/opt/Discord{,PTB,Canary}` via the stable/ptb/canary scripts. Do note that you have to run them as sudo, verify what the scripts do before you run them.

Also change `DATADIR` and `BINDIR` variables before running to match your distros.

```
DATADIR="/usr/share"
BINDIR="/usr/bin"
```

By default, discord{,-ptb,-canary}.desktop is installed in `/usr/share/applications/` and icons are installed to `/usr/share/icons/`.

There is also a `FLAGS` variable to automatically set some flags when launching with the .desktop file, by default `--disable-smooth-scrolling --ozone-platform-hint=auto --enable-experimental-web-platform-features` flags are set.
