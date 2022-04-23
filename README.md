# WineTadah Mac v1.6
Some simple Shell scripts to setup ORC revivals semi-automatically on Linux.

These scripts are not supported in any way, shape or form by the official devs of these revivals.

# What this does
This script will download dependencies, register URI and install the revival of choice. It can also install DXVK, use/make a custom Wineprefix (tadah and placeholder only) and uninstall the revival of choice.

# Dependencies
The needed packages are:
- sudo (installed on most macs)
- The latest wine (get it from)
- wget (also installed on most macs)
- unzip (probably installed on most macs, idk)

If you are running any form of Ubuntu (that includes Linux Mint and PopOS), Manjaro, Fedora or Gentoo the script will automatically install the dependencies for you.

If you aren't, install them manually via your package manager.

# How to use it

0. If your distro is not listed above then install the dependencies.
1. Download the latest release from the Releases page (or just clone this repo via git)
2. Open a terminal and cd into where the script is downloaded.
3. Run `chmod +x *.sh` (which will make all Shell files in that directory executable)
4. Depending on which revival you want to install, run the following commands:
- `./tadah-helper.sh` for Tadah
- `./itteblox-helper.sh` for Itteblox (NOT FINISHED)  
- `./placeholder-helper.sh` for Placeholder (NOT FINISHED)  
5. Once installed, play a game and it should work!

If you want to install DXVK alongside the revival, run the script with the parameter "dxvk".

If you want to use/make a custom Wineprefix alongside the revival, run the script with the parameter "prefix". These two can also be used alongside each other.

If you want to uninstall a revival, run the script with the parameter "uninstall". 

E.g, `./tadah-helper.sh dxvk/prefix/uninstall`

# Troubleshooting
If the game crashes/doesn't launch, try to
1. Run the installer again (make sure you're running it as non-root)
2. Make sure the OS is set to `Windows 10` in `winecfg`
3. Make sure all necessary optional wine dependencies are installed https://wiki.winehq.org/Building_Wine#Satisfying_Build_Dependencies

If those don't work, DM me on Discord: DarDarDar#3429.

# Known issues
Itteblox 2013 studio doesn't work

Itteblox 2016 locks the mouse after either the right mouse button or shift lock is activated 

Placeholder Installer is a bit wonky (uninstaller seems to not work)

(these three are probably unfixable, sadly)

# Credits
calones for helping me, and putting up with me being dumb

thexkey for helping me alot making the Placeholder helper

itteh, kinery and thexkey for making great revivals
