![Babble Logo](https://github.com/san-nyan/images/blob/main/Babble.png?raw=true)

<h3 align="center">
This is san-nyan's fork of <a href="https://github.com/Project-Babble/ProjectBabble">Project Babble</a>
</h3>

<h3 align="center">On this fork the <code>main</code> branch is based off Project Babble's <code>autocalibrator</code> branch so it is based off 2.1.0 RC3</h3>

---

## Changes

- Muted sound effects because they were insanely loud on my system
- Updated requirements.txt to work on linux
- Changed UI colors because I can and I wanted to

---

## Pros

- Your ears will not die if you use Arch Linux
- Larger Monospace font
- Fancy colors wow babble discord server "why does your app look like that"
- If you use this you are 14% cooler
- You can dm me on discord (@__san) for support cause I will think you are 14% cooler instead of being intimidated by messaging a giant discord server

## Cons
- I dont know how to use github but someday I will figure it out so I can keep this updated

---

## Installation

#### The only official way to use this fork is by building it from source

You will need a [Python](https://www.python.org/downloads/) and [pip](https://pip.pypa.io/en/stable/installation/)

##### First clone the repo (or the branch you want) and cd:
```bash
git clone https://github.com/san-nyan/ProjectBabble && cd ProjectBabble/BabbleApp
```
---

##### Make a venv and activate it:
```bash
python -m venv venv && source venv/bin/activate
```
---

##### Install the requirements for your system:
Windows:
```bash
pip install -r requirements-windows.txt
```
Linux:
```bash
pip install -r requirements-linux.txt
```
If you're using this tutorial to install the normal ProjectBabble you should still use one of my requirements files instead of the default included one as it is meant to be modified with a script before ran so go [here](https://github.com/san-nyan/ProjectBabble/tree/main/BabbleApp) and download the requirements file for your system, move it to the ProjectBabble/BabbleApp folder and then run the related above command

---

##### Now you can run the app like this:
```
python babbleapp.py
```

##### For subsequent runs make a script for these commands:
```bash
#!/bin/bash
# cd wherever you installed
cd ProjectBabble/BabbleApp
source venv/bin/activate
python babbleapp.py
```
---


#### Notes on Linux:

##### KDE Plasma

If your GUI window shows just the top row of radio buttons, set a resolution for the Babble App manually in KDE's Window Settings. 800x600y is a good starting point with plenty of empty space.

---

##### v4l2/v4l-linux

If you receive a `["Error listing UVC devices on Linux ... No such file or directory"]` when choosing/changing your camera, you'll need to install video4linux (`v4l-utils`) for your distro.

For Ubuntu or other distros with apt:
```bash
sudo apt-get install v4l-utils
```

---

##### tkinter

If you receive a `ModuleNotFoundError: No module named 'tkinter'` error message on run, you'll need to install `tkinter` for your distro.

For Ubuntu or other distros with apt:
```bash
sudo apt-get install python3-tk
```
For Fedora:
```bash
sudo dnf install python3-tkinter
```
For MacOS:
```bash
brew install python-tk
```

You can read more about this [here](https://stackoverflow.com/questions/25905540/importerror-no-module-named-tkinter) and [here](https://stackoverflow.com/questions/36760839/why-does-python-installed-via-homebrew-not-include-tkinter).
