# xcd

Is an extended **cd** comand, which can store you favourite paths for easy access.

## Usage

    xcd [-a \<path\>[] (-r)

        -a | --add [\<path\>]  Adds path to list of favourite paths.
                               If no path is given the current work dir is used.
        -r | --remove          Removes path from favourites. Will show a selection.
        --setup                Adds an alias for xcd to your .bashrc
        -v | --version         Show version.
        -? | --help            Shows this help.

## Examples

**Tiresome path change**

    user@host:~$ cd /media/disk/projects/local/linux

**Add to favourites**

    user@host:/media/disk/projects/local/linux$ xcd -a
    Added '/media/disk/projects/local/linux'

**Back at home**

    user@host:/media/disk/projects/local/linux$ cd

**Quickly go to something with 'linux' in path**

    user@host:~$ xcd linux
    Filter 'linux'
    [1] /media/disk/projects/local/linux/glight
    [2] /media/disk/projects/local/linux
    Go to: 2
    user@host:/media/disk/projects/local/linux$

**Where was I recently?**

    user@host:~$ xcd

    [G] Go to a location
    [A] Add a location
    [R] Remove a location

    History:
    [1] /media/disk/projects/local/linux
    [2] /media/disk/projects/local/linux/glight
    [3] /home/user
    [4] /media/disk/projects/local/arduino/sketchbooks
    [5] /media/disk/projects/local
    Choose: 1
    user@host:/media/disk/projects/local/linux$

## Background

Favourites and history will be stored in $HOME/.config/xcd

These files will be created automatically.

## License

Copyright (C) 2017  Martin Feil aka. SGDW

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see http://www.gnu.org/licenses/

*Release: Version: 1.0 / Date: 2017-10-12*
