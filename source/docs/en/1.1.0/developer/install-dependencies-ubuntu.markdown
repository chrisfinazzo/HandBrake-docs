---
Type:            article
State:           [ obsolete ]
Title:           Installing dependencies on Ubuntu
Project:         HandBrake
Project_URL:     https://handbrake.fr/
Project_Version: 1.1.0
Language:        English
Language_Code:   en
Authors:         [ Bradley Sepos <bradley@bradleysepos.com> (BradleyS) ]
Copyright:       2024 HandBrake Team
License:         Creative Commons Attribution-ShareAlike 4.0 International
License_Abbr:    CC BY-SA 4.0
License_URL:     https://handbrake.fr/docs/license.html
---

Installing dependencies on Ubuntu
=================================

The following instructions are for [Ubuntu](https://www.ubuntu.com) 18.04 LTS (Bionic Beaver), 16.04 LTS (Xenial Xerus), and Ubuntu 14.04 LTS (Trusty Tahr).

Basic requirements to run commands:

- sudo (for normal user accounts)

Dependencies:

- autoconf
- automake
- build-essential
- cmake
- git
- libass-dev
- libbz2-dev
- libfontconfig1-dev
- libfreetype6-dev
- libfribidi-dev
- libharfbuzz-dev
- libjansson-dev
- libmp3lame-dev
- libogg-dev
- libopus-dev
- libsamplerate-dev
- libtheora-dev
- libtool
- libvorbis-dev
- libx264-dev
- libxml2-dev
- m4
- make
- patch
- pkg-config
- python
- tar
- yasm
- zlib1g-dev

Additional Ubuntu 18.04 LTS and 16.04 LTS dependencies:

- libtool-bin

Graphical interface dependencies:

- intltool
- libappindicator-dev
- libdbus-glib-1-dev
- libglib2.0-dev
- libgstreamer1.0-dev
- libgstreamer-plugins-base1.0-dev
- libgtk-3-dev
- libgudev-1.0-dev
- libnotify-dev
- libwebkitgtk-3.0-dev

Additional Ubuntu 18.04 LTS graphical interface dependencies:

- gstreamer1.0-libav

Install dependencies.

    sudo apt-get update
    sudo apt-get install autoconf automake build-essential cmake git libass-dev libbz2-dev libfontconfig1-dev libfreetype6-dev libfribidi-dev libharfbuzz-dev libjansson-dev libmp3lame-dev libogg-dev libopus-dev libsamplerate-dev libtheora-dev libtool libvorbis-dev libx264-dev libxml2-dev m4 make patch pkg-config python tar yasm zlib1g-dev

If you are running Ubuntu 18.04 LTS or 16.04 LTS, install the additional dependencies.

    sudo apt-get install libtool-bin

To build the GTK [GUI](abbr:Graphical User Interface), install the graphical interface dependencies.

    sudo apt-get install intltool libappindicator-dev libdbus-glib-1-dev libglib2.0-dev libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev libgtk-3-dev libgudev-1.0-dev libnotify-dev libwebkitgtk-3.0-dev

If you are running Ubuntu 18.04 LTS, install the additional graphical interface dependencies.

    sudo apt-get install gstreamer1.0-libav

Ubuntu is now prepared to build HandBrake. See [Building HandBrake for Linux](build-linux.html) for further instructions.
