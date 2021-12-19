# HstWB Mini Package

HstWB Mini is a minimized Workbench setup by Henrik Nørfjand Stengaard targeted A500, A600, A1200 with only chip ram and no fast ram or accelerator card.

It's tailored for harddrive images using FastFileSystem filesystem, but works fine with PFS3 filesystem as well. Note that FastFileSystem filesystem uses ~20 KB of chip ram per partition and PFS3 uses ~300 KB of chip ram per partition, if there is no fast ram installed.

## Description

HstWB Mini package contains following features:

- Minimalistic startup sequence for maximum chip available.
- Boot selectors for starting AGS2 Games and Demos menus, HST Games and Demos menus, DirOpus4, Workbench or CLI.
- Programs installed: DirOpus.

Installation makes following changes:

- Creates backup of startup sequence as "S:Startup-Sequence.BAK".
- Creates backup of user startup as "S:User-Startup.BAK".
- Patch startup sequence and user startup with HstWB changes for best Amiga OS compatibility with existing and future versions.

## Requirements

HstWB Mini package can be installed on any Amiga with Amiga OS 3.2, 3.1.4 or 3.1 about 3MB free space on a harddrive for installation. 

## Installation

HstWB Mini package can be installed using one of the self install images available at https://hstwb.firstrealize.com (recommended) or using install or build self install mode in HstWB Installer (for advanced users).

Use HstWB Installer's update packages to get latest version downloaded automatically.

For manual installation, download latest release from https://github.com/henrikstengaard/hstwb-mini-package/releases and copy it to HstWB Installer "packages" directory.

Then it's ready to be installed using using install or build self install mode in HstWB Installer.

## Assigns

Installation of HstWB Mini package requires and uses following assign and default value:

- SYSTEMDIR: = DH0:

HstWB Mini files will be installed and configured in SYSTEMDIR: assign, which must be set to harddrive containing Workbench.

### Amiga Boot Selector

Amiga Boot Selector is installed with HstWB Mini. It's a fullscreen boot selector with smooth drop in and out effects when loading a selected boot option. It allows selecting boot options using arrow keys and enter or joystick in port 2. Mouse is not supported. 

HstWB Mini is configured with following boot options in Amiga Boot Selector:

1. AGS2Games: Starts AGS2 games menu, if EAB WHDLoad Games menu package is installed.
2. AGS2Demos: Starts AGS2 demos menu, if EAB WHDLoad Demos menu package is installed.
3. HSTGames: Starts HST Launcher menu, if EAB WHDLoad Games menu package is installed.
4. HSTDemos: Starts HST Launcher menu, if EAB WHDLoad Demos menu package is installed.
5. HSTGames1MB: Starts HST Launcher menu, if EAB WHDLoad Games menu package is installed. This menu is filtered with WHDLoad games that should work with only 1MB chip ram.
6. HSTDemos1MB: Starts HST Launcher menu, if EAB WHDLoad Demos menu package is installed. This menu is filtered with WHDLoad demos that should work with only 1MB chip ram.
7. DirOpus4: Starts Directory Opus 4 with compact flash device CF0: mounted for transfering files on A600 or A1200.
8. Workbench: Starts Workbench.
9. CLI: Starts CLI for maximum available memory.

A 5 second timer will automatically select last used boot option, which by default is AGS2Games.

Amiga Boot Selector can be changed by pressing F1. This allows changing existing boot options or add new ones.

## Screenshots

Screenshots of HstWB Mini.

![HstWB Mini 1](screenshots/hstwb-mini_1.png?raw=true)

![HstWB Mini 2](screenshots/hstwb-mini_2.png?raw=true)

![HstWB Mini 3](screenshots/hstwb-mini_3.png?raw=true)

![HstWB Mini 4](screenshots/hstwb-mini_4.png?raw=true)

![HstWB Mini 5](screenshots/hstwb-mini_5.png?raw=true)

![HstWB Mini 6](screenshots/hstwb-mini_6.png?raw=true)

![HstWB Mini 7](screenshots/hstwb-mini_7.png?raw=true)

![HstWB Mini 8](screenshots/hstwb-mini_8.png?raw=true)

![HstWB Mini Amiga OS 3.2](screenshots/hstwb-mini_3.2_1.png?raw=true)

![HstWB Mini Amiga OS 3.1.4](screenshots/hstwb-mini_3.1.4_1.png?raw=true)

![HstWB Mini Amiga OS 3.1](screenshots/hstwb-mini_3.1_1.png?raw=true)