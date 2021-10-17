# NAME

backslide - Change the current desktop wallpaper with a selection from the given path.


# SYNOPSIS

**backslide** [ **-d** _environment_ ] [ **-R** ] [ **-r** ] [ **-l** ] [ **-q** ] _path_...


# DESCRIPTION

**backslide** will parse the folder `path` for image files and changes the current wallpaper.  Currently, JPG and PNG image files are supported.  From the list of wallpapers and the current wallpaper, the script will automatically select the next wallpaper in the list.  If option **-r** is enabled, a random wallpaper is selected.  If option **-l** is enabled, the wallpaper with the latest timestamp is selected.


# OPTIONS

**-d** _environment_
: force setting of wallpaper for specified desktop environment.  If the user has a X session running the value will be detected automatically.  If **backslide** is invoked via a cronjob, this setting is mandatory.  The following settings are supported: "gnome", "mate", and "xfce".

**-R**
: recurse into subfolders when parsing `path` for image files.

**-r**
: select a random image file from the list of wallpaper files.

**-l**
: select the latest file from the list of wallpaper files.

**-q**
: enable quiet mode.

**-h**
: show this help message.


# INSTALLATION

Clone the remote repository and change into the local repository:

```bash
$ git clone https://github.com/mboljen/backslide
$ cd backslide
```

Use the following command to install this software:

```bash
$ make
$ make install
```

The default `PREFIX` is set to `/usr/local`.  In order to successfully complete the installation, you need to have write permissions for the installation location.


# CONTRIBUTION

Pull requests are welcome.  For major changes, please open an issue first to discuss what you would like to change.

Submit bug reports online at: <https://github.com/mboljen/backslide/issues>

Please make sure to update tests as appropriate.


# SEE ALSO

Full documentation and sources at: <https://github.com/mboljen/backslide>


# LICENSE

[MIT](https://choosealicense.com/licenses/mit/)
