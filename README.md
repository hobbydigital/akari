# The Akari Project

The Akari Project is in its infancy. The longterm goal is to build a community and ecosystem around the HD Akari Microcomputer, a modern system that restores the essential features of early micros, like the Beeb and C64.

This repo contains all of the project documentation. You should familiarize yourself with this README, before looking to the wiki for more specific information.

## The Akari Agenda

The Akari uses [modern hardware][1], running [Apex][2], a Linux distibution that is derived from Raspbian Lite. However, the peripherals are fully standardized (a feature we named *holistic standardization*), and the operating system has been extended to support a more traditional paradigm (a feature we named *holistic wizardry*).

Instead of manufacturing the system, the project takes a little inspiration from fantasy consoles (like *PICO-8* and *TIC-80*), and begins by defining an idealized, fictional microcomputer with specs that make it easy and affordable for anyone to cobble together a fully compatible clone from readily available components.

We could have just said that each clone is a clone of all of the other clones, but having a fictional company behind our fictional microcomputer allows us to have fun creating lore and a brand, and gives the community something tangible to indentify with - to put on a sticker. The backstory will be developed openly, so anyone can contribute.


## Holistic Standardization


The [Akari Hardware Specification][1] aims to be as flexible as possible, while still guaranteeing that anything developed by one person will work the same way for every other member of the community.

In simple terms, we specify the board (the *RaspberryPi 3 Model B+*), the resolution of the monitor (1080p), the keyboard layout (ANSI US) and the gamepads (*SN30 Pro* or *SF30 Pro* controllers from 8BitDo).


## Holistic Wizardry

During the eighties, as computer graphics became more affordable, office computers migrated from the old wizardry paradigm to the new desktop paradigm, which has since become the standard interface for all personal computers.

A desktop environment can do a lot that a text based operating system cannot, and you can run an emulator if you need to access the terminal still. It seemed like the best of both worlds. However, early home computers went in a different direction.

The home systems of the eighties simply extended the existing wizardry paradigm with APIs for graphics and audio et cetera. The focus was still oriented around the mastery of arcane languages, collecting libraries and scripts, and issuing shell commands. Cool new features were simply incorporated into the old paradigm. Instead of running programs in little graphical windows, we used APIs to render hardware accelerated graphics directly to the framebuffer, temporarily taking over the terminal, just like a console application does, and importantly, also returning to the terminal once the program exited.

In principle, *any* desktop application could have been implented to be launched from a terminal and rendered fullscreen, without the need for a desktop environment or window manager. Having multiple TTYs also makes it possible to run a handful of graphical applications in parallel, and easily switch between them using keybindings. In fact, if every user of a given operating system is willing to learn basic shell commands, the desktop paradigm is basically redundant.

The HD Akari reintroduces the traditional paradigm. It boots to a `bash` shell, in a `tmux` enhanced TTY, and provides APIs for rendering 2D and 3D graphics to the framebuffer. It also adds APIs for audio, user input and everything else you need to make videogames. The OS also includes libraries that greatly simplify developing advanced shells and console applications.

We contend that the early home micros had the right idea, and that ever more powerful wizardry is the paradigm that actually offers the best of both worlds, while the desktop paradigm only became popular because it is does not require basic computer literacy, which is arguably its greatest weakness.


## Project Status

Again, the project is in its infancy, and the 

[1]: https://github.com/hobbydigital/akari/wiki/The-HD-Akari-Hardware-Specification
[2]: https://github.com/hobbydigital/akari/wiki/The-Apex-Operating-System
