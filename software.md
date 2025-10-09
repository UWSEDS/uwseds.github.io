---
layout: page
title: Software
collection: fall2021
---

The course makes use of a number of software packages that students will install on their computers.
The following software are available for Windows, Mac, and Linux.

**You will need to be connected to `eduroam` WiFi for most of what we want to do in class to work.**

**Please try to install all of this software on your computer before the first day of class.**

## 1. Ensure you have access to a Unix-style terminal.

### macOS and Linux operating systems

Use your operating system's program search (MacOS: spotlight search, Cmd-Space. Ubuntu: Ubuntu button in upper-left corner) up and search for `Terminal`.

You should get a window with a command prompt. Command prompt might have different words / characters, followed by a `$` and cursor for text input. Late 2018 and newer MacOS computers default to `zsh` instead of `bash`. This difference will briefly be covered in class, but you can run `bash` [+ Enter] in the terminal if you choose to use that instead.

### Windows 11 and Windows 10, version 1607+ (Windows Linux Subsystem)

All Windows users should note that the Windows command lines, cmd and PowerShell, differ greatly from the `bash` or `zsh` command prompt that software developers commonly use. From here on out, we will use "terminal" to refer to the Unix-style unless clearly and explicitly stated otherwise.

Note: Windows Linux Subsystem (WSL2, or the older WSL) is preferred over older Git Bash solutions. It's faster, more similar to what you'll see in class and has a more complete set of Unix programs.

Before trying the suggestions below, try opening the Windows Store (from your start menu) and search for Ubuntu 22.04. It will be a free download and installing it "will just work" for most recent versions of Windows 11 on relatively new hardware.

If installing from the Windows Store does not work, we suggest following these instructions for [installing a WSL distribution](https://learn.microsoft.com/en-us/windows/wsl/install).

Some tips:

- We highly suggest using the Ubuntu 22.04 distribution. Ubuntu is one of the more beginner-friendly Linux distros and the instructor is also able to record screen captures for this setup.
- We suggest setting your Linux distribution username and password to match your Windows ones. This will reduce confusion!

## 2. Ensure that Git is installed

Type `git --version` into the terminal. If the terminal prints out any version number, you are successful. For example, my Macbook Pro returns `git version 2.24.1 (Apple Git-126)` and my Windows 10 WSL system returns `s`.

### macOS note

Some students reported an error with `git`

```raw
xcode-select: note: no developer tools were found at
'/Applications/Xcode.app', requesting install. Choose an option
in the dialog to download the command line developer tools.
```

To fix this, do the following:

- Start a new Terminal
- Run the following command: `xcode-select --install`
- Click `Install`
- Click `Agree` to agree to the terms

For more information, [see this link](http://mac-how-to.wonderhowto.com/how-to/install-command-line-developer-tools-without-xcode-0168115/).

## 3. Create a GitHub.com account

Create a GitHub.com account [on the GitHub website](https://github.com/signup). This is a free account. We will discuss more on the Version Control I lecture. You will need to enter your GitHub username into the survey in the welcome email so that we can associate your GitHub username with your UW NetIT.

## 4. Install GitKraken

Please install [GitKraken](https://www.gitkraken.com/), which provides a graphical user-interface to git, while also providing many features that are conducive for collaboration. We suggest that you download it directly from the [downloads page](https://www.gitkraken.com/download) and follow the setup instructions, although you can also use your OS's package manager. For Windows users follow the directions [here](https://www.gitkraken.com/blog/wsl2-and-gitkraken-client) to install GitKraken in WSL2 rather than in Windows.

GitKraken is free to use on public repositories, if the installation process mentions a free trial, that is just for the paid "pro" version which you do not need for this class.

## 5. Installing Python via Anaconda / Miniconda

We recommend that you use the most recent version of Python 3. Slightly earlier versions of Python 3 work as well. There are some differences between Python 2 and Python 3, and many systems only include Python 2.7 as a standard installation. A Python installation for this course will be managed by the conda package management system, described below.

Conda is a system for installing and otherwise managing Python and other software packages. We recommend that you install conda from the open source community managed conda distribution because they offer terms of service that best align with academic research. The installers are available [here](https://github.com/conda-forge/miniforge), scroll down to the **Install** heading and follow the directions for "Unix-like platforms" (Windows users will be installing this using their WSL bash terminal). Let it install in the default location and answer "yes" to the installer question about initializing conda. 

Below are detailed instructions **after** you have installed conda:

1. Update conda's listing of packages for your system: $`conda update conda`
2. Install Jupyter notebook and its requirements: $`conda install jupyter notebook`
3. Test that Jupyter notebooks run using the terminal to start the notebook: $`jupyter notebook`

If everything has worked correctly, it should print a URL to the console that opens an empty notebook. Depending on settings, it may automatically open the notebook server in your default browser.

## 6. Install a terminal text editor \(if you don't already have one!\)

We highly suggest using Nano, an easy to use text editor in the terminal.

You might already have Nano installed. To check, enter $`nano -version` in the Terminal.
If you get a version number back, for example `Nano 8.6`, then you have Nano installed.
Nano is not installed if you get an error message saying: `command not found: nano`.

Note that some users have reported that on Windows using WSL they need to use $`nano --version`
instead.

Note that on macOS, your Nano version will likely return a version of Pico, for example `Pico 5.06`.
For the purposes of this course, Pico and Nano are identical terminal text editors.

### Installing Nano on a Linux operating systems (including WSL on Windows!)

For Ubuntu distributions, try $`sudo apt-get install nano`. For others, $`yum install nano`.

### Installing Nano on the macOS operating system

MacOS doesn't have a pre-installed package manager for their Unix programs. The best option is Homebrew with [full instructions on the website](https://brew.sh/). You can also choose to use [MacPorts](https://www.macports.org/install.php).

Once installed, download Nano with the following command in your terminal:

- `brew install nano` if using Homebrew
- `sudo port install nano` if using MacPorts

## 7. Install Visual Studio Code \(VS Code\)

[Visual Studio Code \(also known as VS Code\)](https://code.visualstudio.com/download) is a graphical code editor that can be customized and extended with a vast library of open-source extensions.
After installing VS Code, install [the Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python) and [the Jupyter extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter).

If you frequently use R, you can install [the R language extension too](https://marketplace.visualstudio.com/items?itemName=REditorSupport.r).
