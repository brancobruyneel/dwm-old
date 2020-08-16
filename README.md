# My personal fork of dwm

## Requirements
In order to build dwm you need the Xlib header files.

## Installation
Edit config.mk to match your local setup (dwm is installed into the /usr/local namespace by default).

Afterwards enter the following command to build and install dwm (if necessary as root):

    make clean install

## Running dwm
Add the following line to your .xinitrc to start dwm using startx:

    exec dwm

In order to connect dwm to a specific display, make sure that
the DISPLAY environment variable is set correctly, e.g.:

    DISPLAY=foo.bar:1 exec dwm

(This will start dwm on display :1 of the host foo.bar.)

In order to display status info in the bar, you can do something
like this in your .xinitrc:

    while xsetroot -name "`date` `uptime | sed 's/.*,//'`"
    do
    	sleep 1
    done &
    exec dwm


## Keybindings
Take a look in config.def.h.

## Patches
* actualfullscreen
* alwayscenter
* attachasideandbelow
* autostart
* bar-height
* bottomstack, centerdmaster, deck, fibonacci
* centeredwindowname
* cyclelayouts
* hide_vacant_tags
* movestack
* pertag
* restartsig
* smartborders
* status2d
* statuscmd
* swallow
* titlecolor

## Screenshots :camera:
![alt text](img/2020-08-16-123504_1920x1080_scrot.png "screen 1")
![alt text](img/2020-08-16-123625_1920x1080_scrot.png "screen 2")
