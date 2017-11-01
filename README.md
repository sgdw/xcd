# xcd

Is an extended **cd** command, which can store your favourite paths for easy access.

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

*Release: Version: 1.0 / Date: 2017-10-12*
