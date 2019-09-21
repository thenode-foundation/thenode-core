
Debian
====================
This directory contains files used to package thenoded/thenode-qt
for Debian-based Linux systems. If you compile thenoded/thenode-qt yourself, there are some useful files here.

## thenode: URI support ##


thenode-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install thenode-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your thenodeqt binary to `/usr/bin`
and the `../../share/pixmaps/thenode128.png` to `/usr/share/pixmaps`

thenode-qt.protocol (KDE)

