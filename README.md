# backslide

This bash script will change the current desktop wallpaper with a random selection from the given path.  The following desktop environments are supported: [Gnome](https:://www.gnome.org/), [Mate](https://www.mate-desktop.org/), and [Xfce](https://www.xfce.org/).

## Installation

Use the following command to install this software:

```bash
$ make
$ make install
```

The default `PREFIX` is set to `/usr/local`.  In order to succesfully complete the installation, you need to have write permissions for the installation location.

## Usage

The following command will parse the folder `path` for image files and changes the current wallpaper.  Currenlty, JPG and PNG image files are supported.  From the list of wallpapers and the current wallpaper, the script will automatically select the next wallpaper from the list.  If the option `-r` is enabled, a random wallpaper is selected.  If the opton `-l` is enabled, the wallpaper with the latest timestamp is selected.

```bash
$ backslide [-d environment] [-R] [-r] [-l] [-q] path...
```

### Options

+ `-d environment`

  Forces setting of wallpaper for specified desktop environment.  If the user has a X session running the value will be detected automatically.  The following desktop environments are supported:

  - `Gnome`
  - `Mate`
  - `Xfce`

  This setting is mandatory if the script is invoked via a `cron` job.

+ `-R`

  Recurses into subfolders when parsing `path` for image files.

+ `-r`

  Selects a random image file from the list of wallpaper files.

+ `-l`

  Selects the latest file from the list of wallpaper files.

+ `-q`

  Quiet mode.

+ `-h`

  Shows this help message.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
