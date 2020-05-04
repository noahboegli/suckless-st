# Fork notes
Suckless'st fork with some patches applioed.   
If you use this fork, remove `config.h` and generate your own otherwise you might have issue with fonts.  
Last updated: 04.05.2020 (st v0.8.3)  
Applied patches:  
- Scrollback
	- keyboard scroll
	- mouse scroll
	- altscroll   
- Appearance
	- Font 2 (experimental)

# st - simple terminal
st is a simple terminal emulator for X which sucks less.


# Requirements
In order to build st you need the Xlib header files.


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

