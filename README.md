KeepWiFiOn
==========

On OS X, if Wi-Fi gets turned off, then automatically turn it back on.

## What's the point of this?
Mac OS X Mavericks created a small problem for some users of antiquated MacBook Pros: when Wi-Fi gets turned off, the computer freezes within a few minutes.  Rebooting does not help, because upon boot, the computer checks the Wi-Fi state, sees that it's off, and freezes again.

KeepWiFiOn prevent your computer from freezing by

1. Turning Wi-Fi on automatically every time your computer boots
2. Monitoring the status of Wi-Fi during regular computer usage, and forcing Wi-Fi back on whenever it gets turned off

There is usually a delay of at least a couple seconds between turning Wi-Fi off and the computer freezing, so KeepWiFiOn should have enough time to get in there and save your computer.

## Installation

#### Option 1 (simplest):

1. Download the file install_KeepWiFiOn to ~/Downloads
2. Open Terminal and run the command `~/Downloads/install_KeepWiFiOn`

Step 2 will download all the program files from this GitHub repository and install them.

### Option 2 (slightly less simple):

1. Download the following files to ~/Downloads:
  * install_KeepWiFiOn
  * local.KeepWiFiOn.Daemon.plist
  * local.KeepWiFiOn.Agent.plist
  * turn_on_wifi
2. Open Terminal and run the command `~/Downloads/install_KeepWiFiOn --local`

In this case Step 2 will use the files you already downloaded.  Note that all 4 downloaded files must be in the same directory (e.g. ~/Downloads).
