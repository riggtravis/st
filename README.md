st - simple terminal... With simple patches!
============================================
Don't worry... Below you will find the original ST README for the sake of being
a decent citizen. I just have some front matter to get through first for the
sake of explaining why this repository even exists. I wanted to make it easier
to apply patches than what the original suckless project's guidance for hacking
provides. The process to follow is to create a branch for your preferences, and
then merge the patched branches you want into your personal branch. After that
you can just follow the usual ST build process.

Original README follows
=======================
A little more front matter... I've edited the original README slightly to
leverage a few markdown features that should make quality of life better.

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

```sh
make clean install
```


Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

```sh
tic -sx st.info
```

See the man page for additional details. If you are unfamiliar with man pages,
this can be done using the following command:

```sh
man st
```

Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

