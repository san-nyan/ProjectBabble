![Babble Logo](https://github.com/san-nyan/images/blob/main/Babble.png?raw=true)

<h3 align="center">
This is san-nyan's fork of <a href="https://github.com/Project-Babble/ProjectBabble">Project Babble</a>
</h3>

### The current version this supports is 2.0.7 on the `main` branch and 2.1.0 RC3 on the `autocalibrator` branch

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
or
```bash
git clone --branch <branch> https://github.com/san-nyan/ProjectBabble && cd ProjectBabble/BabbleApp
```

##### Make a venv and activate it:
```bash
python -m venv venv && source venv/bin/activate
```

##### Install the requirements for your system:
```bash
pip install -r requirements-windows.txt
```
or
```bash
pip install -r requirements-linux.txt
```

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
