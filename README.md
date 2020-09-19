# dotfiles
My Dotfiles For An OpenBSD rice.

## What Is This?
For the sake of simplicity in transferring my configuration to my other OpenBSD laptops, I finally decided on hosting my dotfiles on git. This allows me to just copy and move a few files, and be "off to the races"

## What's included?
These dotfiles include a riced Xdefaults for `rxvt-unicode` and `rofi`, a default wallpaper, and configuration for the Xenocara X11 fork.

## What software is needed to make it look right?
These dotfiles rely on the packages `urxvt` and `rofi` to function properly, along with a working X11 installation (or Xenocara).

## Installation
First off, copy the `userconfig/Xdefaults` file to your home directory and rename it to `.Xdefaults`. Next, copy the wallpaper to your Pictures folder. If on OpenBSD, replace the files located at `/etc/X11/xenodm/` with the contents repo's xenocara folder. Lastly, extract the `dwm.tar` file, and open a terminal as root user in the `dwm` folder it creates. Then, execute the command `make`. When complete, copy the dwm executable file it created to `/usr/local/bin`. With that, the rice is completely installed.
