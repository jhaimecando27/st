# st - simple terminal (0.9)
st is a simple terminal emulator for X which sucks less.


# Requirements
In order to build st you need the Xlib header files. (the font is optional make sure to change it in config file)

## Ubuntu
```sh
apt install libx11-dev libxft-dev fonts-jetbrains-mono
```

## Fedora
```sh
dnf install libX11-devel libXft-devel jetbrains-mono-fonts
```


# Installation
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


# Running st
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

# Credits
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

