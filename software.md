---
layout: page
title: Software
collection: main
---

The course makes use of a number of software packages that students
will install on their computers.
The following software are available for Windows, Mac, and Linux.

## git and github
git is a system used for version control and collaboration.
You should have a github account and ensure that
git is installed on your computer.

## Bash shell and git software version control
The bash shell provides a programming environment that
is often used to manipulate files, install programs, and
basic data analysis.
The git version control system (along with the github website)
are widely used for sharing codes and collaborative development
of software.
Bash and git are part of Linux and Mac OSX.
Windows users should install gitbash. (See https://git-scm.com/download/win.)
Look [here](https://github.com/UWSEDS/uwseds.github.io/blob/master/software_windows_texteditor.md)
for more
details on the use of an editor with Windows for git.

### Mac OSX note: Some students reported an error with ``git``:
```
xcode-select: note: no developer tools were found at '/Applications/Xcode.app', requesting install. Choose an option in the dialog to download the command line developer tools.
```
To fix this, do the following:

* Start a new Terminal
* Run the following command: ``xcode-select --install``
* Click ``Install``
* Click ``Agree`` to agree to the terms
For more information see this [link](http://mac-how-to.wonderhowto.com/how-to/install-command-line-developer-tools-without-xcode-0168115/)

### Windows user note:
Windows users should install the Software Carpentry recommended software:
Please follow these instructions on YouTube: [https://www.youtube.com/watch?v=339AEqk9c-8](https://www.youtube.com/watch?v=339AEqk9c-8).
Make sure you install gitbash _and_ the text editor (SWCarpentryInstaller).
Links to the installers for Windows:
* GitBASH: [https://git-for-windows.github.io](https://git-for-windows.github.io)
* Software Carpentry Installer: [https://github.com/swcarpentry/windows-installer/releases/](https://github.com/swcarpentry/windows-installer/releases/)


## Get the class notes
Use git to clone the repo for the lectures. (We're assuming that you git installed.)

- git clone https://github.com/UWSEDS/LectureNotes.git

## Python
We recommend that you use Python 3.5. Earlier versions of Python 3 work as well.
There are some differences between Python 2.7 (and earlier releases of Python 2)
and Python 3.
Details on installing Python can be found at https://www.python.org/downloads/.

## Conda
Conda is a system for installing and otherwise managing python packages.
We recommend students use miniconda.
See http://conda.pydata.org/miniconda.html
for instructions for downloading and installing miniconda. 
(You should use the instructions for your OS and Python 3.5.)
Below
are detailed instructions after you have installed miniconda:

1. Update conda's listing of packages for your system:
- $conda update conda
2. Shift to a python 3.5 installation for your system:
- $conda install python=3.5
3. Install IPython notebook and all its requirements:
- $ conda install ipython-notebook
4. Navigate to the directory containing the course material. For example:
- $ cd ~/LectureNotes/02-Python-and-Data
5. Type ipython notebook in the terminal to start the notebook;
- $ ipython notebook

If everything has worked correctly, it should automatically launch your default browser

## Text editor
Students will select a text editor of their choice, such as
Notebook (Windows), vim (all platforms), and sublime (all platforms).
A text editor is different from word processing programs,
like MS Word, in that text editors often recognize
program syntax and do no formatting.



If you don't already have a favorite text editor, we recommend installing either [atom](http://atom.io/) or [Sublime](http://www.sublimetext.com/), which are both available for all platforms.
