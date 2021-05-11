# My build of slock

The suckless [simple X display locker](https://tools.suckless.org/slock/)
with some patches and modifications applied by me.

## Patches

To this build I have applied the following patches:

* [blur pixelated screen](https://tools.suckless.org/slock/patches/blur-pixelated-screen/)

## Requirements

In order to build slock you need the Xlib header files. In addition, the
blur pixelated screen patch requires `imlib2` to be installed.


## Installation

Edit `config.def.h` to your liking, making sure to set appropriate values
for the `user` and `group` variables, otherwise `slock` will error out.
Also, edit `config.mk` to match your local setup (`slock` is installed into
the `/usr/local` namespace by default).

Afterwards run the following command to build and install `slock`

    sudo make clean install

## Running slock

Simply invoke the `slock` command. To get out of it, enter your password.
