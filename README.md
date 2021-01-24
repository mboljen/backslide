# backslide

This bash script will change the current desktop wallpaper with a random selection from the given path.  The following desktop environments are supported: Gnome, Mate, and XFCE.

## Installation

Use the following command to install this software:

```bash
$ make
$ make install
```

The default `PREFIX` is set to `/usr/local`.  In order to succesfully complete the installation, you need to have write permissions for the installation location.

## Usage

The following command :

```bash
$ backslide [-options] path
```

### Options

+ `-d` Force desktop environment (`GNOME`, `MATE`, `XFCE`)
+ `-r` Recurse into subfolders
+ `-n` Random selection
+ `-h` Show this help message

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
