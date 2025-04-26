# Consistent Development Environment across Windows and MacOS 
While carrying out assignments for my Masters Degree, I was split with working between a Macbook M1 Pro and a Windows 11 workstation. I wanted a consistent working environment so that both systems could be used in a similar way. 
For compatibility purposes and also for library availability on Windows it will be setup using Windows subsystem for Linux, which is a mature kernel level extension that allows an Ubuntu installation to be used without dual booting.
Mostly I am developing in Python using VSCode or Jupyter Lab.

The shown with instructions for Windows and Macos. 
The following steps will be done.
1. Install terminal
1. Install Ubuntu or brew package manager
1. Setup zsh and customise with Ohmyzsh
1. Install customised terminal fonts
1. Install git
1. Setup Eza replacement for ll/ls
1. Setup miniforge for Python management using mamba
1. Install VSCode and extensions

The end results will be a git aware visually useful terminal with a couple of expanded tool replacing ls and cat.
<img width="1067" alt="image" src="https://github.com/user-attachments/assets/62f1d619-8c13-453a-989a-86b9b9a80de0" />


## Install terminal
### Windows
Use the windows terminal, if not alread installed you can load it from the app store here.
[Windows Terminal](https://apps.microsoft.com/detail/9N0DX20HK701?hl=en-us&gl=GB&ocid=pdpshare!)

### MacOS
For macos iTerm2 is the preffered choice, however any terminal should work.
To install iTerm2 enter the following command in any terminal

`brew install iterm2`

## Install zsh and ohmyzsh customisation


zsh and customisation using ohmyzsh.
console command eza in place of ll
Open Windows Terminal, if not installed then install it from windows store. 

wsl should be already installed if on windows 11.
list the online distros you can install
wsl --list --online
then install the latest Ubuntu
wsl --install -d Ubuntu-24.04
This will then go through the installation process.
Install Visual Studio Code from the Microsoft Store
now to install some stuff in wsl.
In Terminal open an Ubuntu shell
carry out general updates

---

sudo apt update
sudo apt upgrade
Install miniforge https://github.com/conda-forge/miniforge
Remember to say yes at the end to add shell privileges
in base environment  update using mamba, you can use mamba in place of conda in most call, mamba is superior for package resolution.
mamba update --all

---

I used this as a reference https://dev.to/darraghor/consistent-modern-shell-tooling-on-macos-and-windows-wsl-for-developers-a92

---
