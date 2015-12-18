# README.md
# PhoPlay - Simple audio player
Copyright (c) <2012, 2015> Ben Sampson All rights reserved.

Phoplay is a simple audio player written in Python3 and uses the PyQt4 Phonon
library to provide playback facilities.

It can be invoked as a GUI (default) or from the commandline with or without
the GUI functionality.

## Installation
Running the ./build.sh script will build the QtDesigner resource file and 
UI for the application generated from the QtDesigner .ui file.  If ./build.sh
fails then check that you have PyQt4 installed and the pyrcc4 and py3uic4 are
installed (they may have different names under different Linux distributions)

On opensuse platforms python-qt4-utils provides pyrcc4, python3-qt4-devel 
provides py3uic 

## Usage
A full list of commandline options can seen by invoking the application with
the -h option.

## Examples
```PhoPlay.py - Lauch the GUI```

```PhoPlay.py something.flac``` - Launch GUI and play something.flac

```PhoPlay.py -x something.mp3``` - Play something.mp3 from the commandline - no GUI

Play all mp3s re-launching the application each time.
Useful for playing a album in a folder.

```for tune in *.mp3; do PhoPlay.py -q $tune; done;``` 