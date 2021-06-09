# PIA 

This workflow allows you to interface with the PIA VPN. You must have PIA VPN installed and `piactl` located at `/usr/local/bin/piactl` (which is the default location anyway).

## Usage

This workflow uses `piactl` command-line tool that comes alongside the PIA VPN Application. If you're logged in there, then you don't need to login using this. 

`pia-auth`

If you aren't logged in, use `pia-auth username:password`. This will authenticate you and allow you to connect to the VPN. 

*NOTE: This writes the credentials to disk, as required by `piactl` at `/tmp/piaLogin.txt`. This gets deleted after use, but it's just to let you know.*

`pia-c`

To connect to a region, use `pia-c`. The available options are:

- `auto`		- Connect to the best region, as determined by PIA
- `region`	- e.g 'uk-manchester'
- none		- By passing no argument, this will connect you to the last region connected to.

`pia-dc`

This will disconnect you from the VPN.

`pia-logout`

This will log you out of the VPN. NOTE: This will also log you out of the GUI.
