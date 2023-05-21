# osu!
Keep in mind that the package is **not** official, there may be bugs specific to the flatpak. If you find such, report them here.
> Note: This is osu!(lazer) - a future update which is yet to be considered mainstream. It is not osu!(stable).

## Where is the game directory located?
Check `~/.var/app/sh.ppy.osu/data/osu`

## Graphics tablets
osu! uses [OpenTabletDriver](https://github.com/OpenTabletDriver/OpenTabletDriver) for graphics tablets support.
Refer to their [installation instructions](https://opentabletdriver.net/Wiki/Install/Linux).

Typically, installing it according to their instructions will be enough, but if this does not work, you might need 
to [update your udev rules](https://opentabletdriver.net/Wiki/FAQ/Linux#fail-device-streams).

If all else fails, refer to your distribution's respective help channels.

Please, share your experience of using a graphics tablet in **osu!**. Both on the build in `flatpak` and on the official one (`AppImage`).

## When selecting files, not all directories are visible
This happens because when a flatpak container is launched, only the necessary directories are passed through to it.

If you want to be able to access all files and directories in your home directory, use `Flatseal` from `flatpak`, or `sudo flatpak override sh.ppy.osu --filesystem=home`
