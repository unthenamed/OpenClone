# OpenClone
OpenWrt WWAN Mac address Spoofing

### Purpose
This script spoof a list MAC address for the WWAN interface on an OpenWRT/LEDE router. It is implemented as an [init script](https://wiki.openwrt.org/doc/techref/initscripts), so it is able to spoof the MAC address every the router no internet..

### Dependencies
Nothing special. It should work on a base OpenWRT/LEDE system.

### Usage
1. Copy `openclone` to `/etc/init.d/`
2. Edit list mac addrese in script
3. Make sure the file is executable (`chmod +x /etc/init.d/openclone`)
4. Modify the `START` line in the file if you'd like to customize the init order (optional)
5. Enable the service so it will randomize the MAC address on every boot (`/etc/init.d/openclone enable`)
6. Restart your router or start the service manually (`/etc/init.d/openclone start`)
