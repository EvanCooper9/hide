# clean
quickly &amp; easily hide/show the contents of a directory

## Demo
<p align="center">
  <img src="clean_demo.gif"/>
</p>

## Installation
### [Download](https://github.com/EvanCooper9/clean/archive/master.zip)
```
wget https://github.com/EvanCooper9/clean/archive/master.zip
```

### PATH
 * Place in desired directory
 * Add to your .bash_profile : `PATH=$PATH:/full/path/to/clean`

### Setup
```
clean
> Thank you for installing Clean!
> Would you like to enable Auto Clean (y/n)? y
> What directory would you like to Clean ~/Desktop
```

## Usage
```
clean [-s] | [-h] | [-d DEST] | [-D] | [-a] | [-A] | [-i] | [-r]
```

### Options
  * `-s` Show the files of the current profile
  * `-h` Hide the files of the current profile
  * `-d DEST` Change the current destination. Where `DEST` is the destination to clean
  * `-D` Show the current destination
  * `-a` Enable/disable Auto Clean: show/hide based on the current state
  * `-A` Show if auto clean is enabled/disabled
  * `-i` Show clean info page (Only really useful when Auto Clean is enabled)
  * `-r` Restore Clean to defaults

## Features
### Auto Clean
Auto clean eliminates the need for the `-s` and `-h` flags. It will automatically hide/show the files from the current destination based on the current state. Simple type `clean` and the rest will be taken care of.

### Ignoring files
To have clean ignore files, add the `IGNORE` array variable to the `CONFIG` file. Adding multiple files/directories is easy.
```
# CONFIG
...
IGNORE[0]="file1.png"
IGNORE[1]="file2.txt"
...
```
