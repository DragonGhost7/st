# st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.

I have forcefully applied several patches, all of which you can find in the `patches` directory.

I think these are all. I might have deleted some. Just git diff the whole thing against the `master`, check whats missing.

**Word of caution, this will probably break**

## Requirements
------------
In order to build st you need the Xlib header files.


## Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


## Running st
----------

Its all in the [dwm](https://github.com/DragonGhost7/dwm) config.h, check my build.

## Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

