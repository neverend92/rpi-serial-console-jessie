# rpi-serial-console-jessie
Script to enable/disable the serial console on Raspberry Pi using Rasbian Jessie.

Since the update from Rasbian Wheezy to Rasbian Jessie a few changes where made concering the inittab file, the old approaches to enable/diable the serial console won't work anymore.

So this project is based on [rpi-serial-console](https://github.com/lurch/rpi-serial-console) and is replacing it.

## Installtion
Very similiar to [rpi-serial-console](https://github.com/lurch/rpi-serial-console), simply run:
```
sudo wget https://raw.githubusercontent.com/neverend92/rpi-serial-console-jessie/master/rpi-serial-console-jessie -O /usr/bin/rpi-serial-console-jessie && sudo chmod +x /usr/bin/rpi-serial-console-jessie
```

## Usage
There are three different possible actions:
```
sudo rpi-serial-console-jessie [enable/disable/status]
```

## Advanced Usage
It is also possible to specify the baud rate which should be set when enabling/disabling the serial console:
```
sudo rpi-serial-console-jessie [enable/disable] <baudrate>
```

## Troubleshooting
This script is only tested on Rasbian Jessie, so it might not work on other systems.
If you find a bug, please feel free to open an issue on that.
Tested on Raspberry Pi 2 Model B and EnOcean Pi TCM310.
