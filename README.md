# Mechanica Advisor for Windows

[Download the latest Windows installer](https://github.com/riverkusmon/mechanica-advisor-releases/releases/latest/download/Mechanica-Advisor-Setup.exe)

Mechanica Advisor shows shop questions and estimates above your shop software.
This repository contains the generic Windows x64 installer and signed update
metadata. Shop connection details are supplied separately.

## Install once

1. Download and run the installer under the Windows account used at the counter.
2. Open Mechanica Advisor and enter the server address and connection code supplied
   by your Mechanica contact. Keep that code private.
3. Leave **Start with this computer** and **Update automatically when idle** enabled
   in the tray menu.

For an existing installation, run the new installer over the current app. Keep
its existing data and settings; uninstalling first is unnecessary.

## Automatic updates

Advisor checks after startup and every six hours. It downloads and verifies
updates in the background. Once the Windows session has been idle for five
minutes and no answer or setup form is open, it installs and restarts itself.
No Install click, SSH access or GitHub account is required. It preserves the shop
connection and saved settings. The computer itself does not restart.

**Later** postpones an update for a day. The tray menu also has a manual update
check and an option to turn automatic installation off.

Updates are verified using Mechanica's updater signing key. Windows publisher
signing is not yet configured, so Windows may show an unknown-publisher warning
for the first installation. If your organization's controls block installation,
contact your Mechanica contact or IT administrator.
