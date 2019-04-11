# The Akari Project

The Akari Project is in its infancy. The longterm goal is to build a community and ecosystem around the HD Akari microcomputer, a modern system that restores the essential features of early micros, like the Beeb and C64. This repo contains the project documentation.

The Akari uses [modern hardware][1], and its [Apex operating system][2] is derived from Raspbian Lite, but the peripherals are standardized like an early micro, and the operating system has been extended to support a more traditional paradigm.

Instead of manufacturing the system, the project instead defines an idealized fictional microcomputer, with specs that make it easy and affordable for anyone to cobble together a fully compatible clone from readily available components.

The [Akari Hardware Specification][1] aims to be as flexible as possible, while still guaranteeing that anything developed by one person will work the same way for every other member of the community. In simple terms, we specify the board (the *RaspberryPi 3 Model B+*), the resolution of the monitor (1080p), the keyboard layout (ANSI US) and the gamepads (one to four 8BitDo *SN30 Pro* or *SF30 Pro* controllers).

## The Akari Paradigm

As computer graphics became more affordable, it allowed office computers to move from the old wizardry paradigm to a desktop paradigm, which has become the standard interface for all personal computers.

A desktop environment can do a lot that a text based operating system cannot, and you can run an emulator if you need to access the terminal still. It seemed like the best of both worlds. However, early home computers tried a different approach.

The early home systems simply extended the existing wizardry paradigm with APIs for graphics, audio et cetera. The focus was still oriented around the mastery of arcane languages, collecting libraries and scripts, and issuing shell commands, and cool new features were simply incorporated into the old paradigm. Instead of running programs in little graphical windows, we used APIs to render hardware accelerated graphics directly to the framebuffer, temporarily taking over the terminal, just like a console application does.

In principle, *any* desktop application could have been implented to be launched from a terminal and rendered fullscreen, without the need for a desktop environment or window manager. Having multiple TTYs also makes it possible to run a handful of graphical applications in parallel, and easily switch between them. In fact, if every user of a given operating system was willing to learn basic shell commands, the desktop paraigm would offer nothing unique, and completely lacks the power and freedom that languages offer.

The HD Akari reintroduces the traditional paradigm. It boots to a `bash` shell, in a `tmux` enhanced TTY, and provides APIs for rendering 2D and 3D graphics to the framebuffer. It also adds APIs for audio, user input and everything else you need to make videogames, as well as libraries that help with developing advanced shells and console applications.

We contend that the early home micros had the right idea, and that enhanced wizardry is the paradigm that offers the best of both worlds, while the desktop paradigm only became popular because it is does not require basic computer literacy, which is not a strength.

[1]: https://github.com/hobbydigital/akari/wiki/The-HD-Akari-Hardware-Specification
[2]: https://github.com/hobbydigital/akari/wiki/The-Apex-Operating-System
