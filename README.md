# gw's custom st build
All patches in the `patches` directory are already preapplied to the build. There is no need to apply any of the aforementioned patches to the build yourself. I strongly advise against it.
This build uses the `st-xresources` patch, as such there is no need to interact with the source code to change most basic things. To see which changes can be applied through .Xresources, refer to `config.def.h`.

# Default st README
st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.


Requirements
------------
In order to build st you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

