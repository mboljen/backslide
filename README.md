# backslide

Change the current desktop wallpaper with a selection from the given path.


## Description

**backslide** will parse the folder `path` for image files and change the current wallpaper.  Currently, JPEG and PNG files are supported.  From the list of wallpapers found and the current wallpaper, **backslide** will automatically select the next wallpaper in the list.  If option **-r** is enabled, a random wallpaper is selected.  If option **-l** is enabled, the wallpaper with the latest timestamp is selected.


## Synopsis

```console
$ backslide [OPTION]... PATH...
```

## Options

+ **-d** _environment_

  Force setting of wallpaper for specified desktop environment.  If the user has a X session running the value will be detected automatically.  If **backslide** is invoked via a cronjob, this setting is mandatory.  The following settings are supported: "gnome", "mate", and "xfce".

+ **-R**

  Recurse into subfolders when parsing `path` for image files.

+ **-r**

  Select a random image file from the list of wallpaper files.

+ **-l**

  Select the latest file from the list of wallpaper files.

+ **-q**

  Enable quiet mode.

+ **-h**

  Show this help message.


## Installation

Clone the remote repository and change into the local repository:

```console
$ git clone https://github.com/mboljen/backslide
$ cd backslide
```

Use the following command to install this software:

```console
$ make
$ make install
```

The default `PREFIX` is set to `/usr/local`.  In order to successfully complete the installation, you need to have write permissions for the installation location.


## Contributing

Pull requests are welcome.  For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.


## License

[MIT](https://choosealicense.com/licenses/mit/)
