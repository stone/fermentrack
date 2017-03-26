# Armbian
This guide should be good for almost any of the modern boards with Armbian.
Armbian is a lightweight Debian/Ubuntu based distribution specialized for 
ARM developing boards. Compiled from scratch.

Armbian Supports a wide variety of [boards](http://www.armbian.com/download/) like

- Orange Pi One/Zero/PC/PC2...
- Tingerboard
- Pine64
- Banana Pi

# Preparing a Orange Pi One for Fermentrack

Prior to installing Fermentrack, you need to install Armbian and setup networking.

### Prepare the Raspberry Pi

1. Download the latest version of Armbian from [here](https://www.armbian.com/orange-pi-one/). I recommend the Server version as I prefer headless installations, but the Desktop version works as well.
1. Write the Armbian image to a good reliable SD card, I recommend [Etcher](https://www.etcher.io/) witch is a multi platform image writer.
1. Plug the SD card into your Orange Pi, connect the Orange Pi to ethernet and plug in power.
1. Locate the IP address for your Orange Pi This can generally be done by executing `arp -a | grep armbian` however you can also locate your Orange Pi by logging into your router and looking for the device.
1. Login as root over ssh with password 123, you will be asked to change it.
1. Configure wifi if needed, nmtui-connect
1. Update the Orange Pi software by running `sudo apt-get update` and `sudo apt-get upgrade`.

For more information consule the [Armbian Documentation](https://docs.armbian.com/)