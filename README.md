# isodrive (configfs)

## Building

* `sudo apt install build-essential`

* `git clone https://github.com/furilabs/isodrive`

* `cd isodrive`

* `make`

* `sudo make install` (optional)

## Usage
```bash
Usage:
isodrive [FILE]... [OPTION]...
Mounts the given FILE as a bootable device using configfs.
Run without any arguments to unmount any mounted files and display this help message.

Optional arguments:
-rw		Mounts the file in read write mode.
-cdrom		Mounts the file as a cdrom.
-configfs	Forces the app to use configfs.
-usbgadget	Forces the app to use sysfs.
```

### Examples

mount iso as rw
```bash
isodrive /path/to/file.iso -rw
```

mount iso as cdrom
```bash
isodrive /path/to/file.iso -cdrom
```
