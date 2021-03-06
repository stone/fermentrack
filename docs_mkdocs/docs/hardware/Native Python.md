# Fermentrack and Fuscus (Native Python Controller)

As of now, serial connections are supported by Fermentrack, and therefore it is expected that Fuscus should be Fermentrack compatible. Fuscus support *has not been tested* and should be considered experimental.

Due to the nature of the serial ports used by Fuscus, the serial autodetection process cannot be used to set up a Fuscus-based controller. Connections to Fuscus can be set up using the ["advanced" workflow](../config/Advanced%20Controller%20Setup.md) and manually specifying the Fuscus serial port. 

**NOTE** - If setting up a Fuscus-installation manually, make sure to set "prefer_connecting_via_udev" to False. If this is true, BrewPi-Script may either not connect or connect to the wrong device.

Further down the development path are other features involving Fuscus such as direct installation and configuration management - though these are expected in v3 and beyond.
