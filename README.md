# arrismon
Asuswrt-Merlin Addon for Arris SURFboard SB61XX Modems

## About
arrismon is a tool that tracks your cable modem's stats (such as signal power levels) for AsusWRT Merlin with charts for daily, weekly and monthly summaries. 
It is mostly identical to modmon created by JackYaz. However, arrismon is customized for another series of modems, the Arris SURFboard SB61XX line.
It likely wont work with the newer DOCSIS 3.1 modems (i.e. SB8200 series). Im sure it can be adapted but I don't have access to one to parse it's html logs.
@WRKDBF-Guy added login/credential management for Arris modems that require a login to retrieve stats.


arrismon is free to use under the [GNU General Public License version 3](https://opensource.org/licenses/GPL-3.0) (GPL 3.0).

## Installation

Using your preferred SSH client/terminal, copy and paste the following command, then press Enter:

/usr/sbin/curl --retry 3 "https://raw.githubusercontent.com/JGrana01/arrismon/master/arrismon.sh" -o "/jffs/scripts/arrismon" && chmod 0755 /jffs/scripts/arrismon && /jffs/scripts/arrismon install
## Usage
### WebUI
arrismon can be configured via the WebUI, in the Addons section. I recommend you use USB and not JFFS, in those settings. See the statement from RMerlin at https://github.com/RMerl/asuswrt-merlin.ng/wiki/JFFS.

### Command Line
To launch the arrismon menu after installation, use:
```sh
arrismon
```

If this does not work, you will need to use the full path:
```sh
/jffs/scripts/arrismon

