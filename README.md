KeepWiFiOn
==========

On OS X, if Wi-Fi gets turned off, then automatically turn it back on.

## What's the point of this?
Mac OS X Mavericks created a small problem for some users of antiquated MacBook Pros: when Wi-Fi gets turned off, the computer freezes within a few minutes.  Rebooting does not help, because upon boot, the computer checks the Wi-Fi state, sees that it's off, and freezes again.

KeepWiFiOn prevents your computer from freezing by:

1. Turning Wi-Fi on automatically every time your computer boots
2. Monitoring the status of Wi-Fi during regular computer usage, and forcing Wi-Fi back on whenever it gets turned off

There is usually a delay of at least a couple seconds between turning Wi-Fi off and the computer freezing, so KeepWiFiOn should have enough time to get in there and save your computer.

KeepWiFiOn is only a band-aid solution, as it does not fix the underlying issue of why turning Wi-Fi off freezes the computer for some users.  Perhaps only Apple can address that, but in the meantime KeepWiFiOn can spare you some frustration.

## Installation

#### Option 1 (simplest):

1. Download the file [install_KeepWiFiOn][installer] (right click and save link target) to ~/Downloads
2. Open Terminal and run the command `~/Downloads/install_KeepWiFiOn`

Step 2 will download all the program files from this GitHub repository and install them.  After that you can delete the installer if you'd like.

#### Option 2 (slightly less simple):

1. Download the following files to ~/Downloads:
  * [install_KeepWiFiOn][installer]
  * [local.KeepWiFiOn.Daemon.plist][daemon]
  * [local.KeepWiFiOn.Agent.plist][agent]
  * [turn_on_wifi][script]
2. Open Terminal and run the command `~/Downloads/install_KeepWiFiOn --local`

In this case Step 2 will use the files you already downloaded.  Note that all 4 downloaded files must be in the same directory (e.g. ~/Downloads).  After installing you can delete all the downloaded files if you'd like.

The advantage of Option 2 is that if something goes wrong during installation, you can try again without having to redownload the files every time.

## Uninstallation

1. Down the file [uninstall_KeepWiFiOn][uninstaller] to ~/Downloads
2. Open Terminal and run the command `~/Downloads/uninstall_KeepWiFiOn`

Note that the uninstaller will only attempt to remove files created by the installer, not files that you downloaded.

## Disclaimer

This software is meant to be run on OS X Mavericks (and maybe later OSes, if the Wi-Fi bug persists).  I have only tested KeepWiFiOn on my computer, a MacBook Pro 17" from late 2007, running OS X 10.9.4.  I obviously cannot guarantee that it will work for you.  If you do encounter any issues, please [let me know][issue].

[installer]: https://raw.githubusercontent.com/dmuenz/KeepWiFiOn/master/install_KeepWiFiOn
[uninstaller]: https://raw.githubusercontent.com/dmuenz/KeepWiFiOn/master/uninstall_KeepWiFiOn
[daemon]: https://raw.githubusercontent.com/dmuenz/KeepWiFiOn/master/local.KeepWiFiOn.Daemon.plist
[agent]: https://raw.githubusercontent.com/dmuenz/KeepWiFiOn/master/local.KeepWiFiOn.Agent.plist
[script]: https://raw.githubusercontent.com/dmuenz/KeepWiFiOn/master/turn_on_wifi
[issue]: https://github.com/dmuenz/KeepWiFiOn/issues/new
