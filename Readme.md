# WipeDisk

WipeDisk is a Debian Linux live-build formula and accompanying BASH script to
facilitate disk wiping (overwriting by \x00) of devices connected to the system.
It will boot in 64-bit UEFI systems (modern Windows PCs and Intel Macs) and has
a modern kernel with drivers to access NVMe SSD drives.

## Features

WipeDisk is console-only so, there are no graphics card conflicts.  It boots
straight to the application, and quitting the application causes the system to
shutdown.

The ISO label "WipeDisk" is used to prevent the WipeDisk device from listing
itself as a wipe candidate thus preventing the WipeDisk device from wiping
itself.

WipeDisk requires an affirmative choice to wipe a device, meaning that the user
cannot accidentally wipe a device by accepting default menu selections.

## WIP

WipeDisk is a work in progress.  It was built to make it easy for users to wipe
internal devices and any attached external devices before recycling a device.
It currently only allows the wiping of one device at a time and doesn't provide
verification (which would double the wait time).  Future versions may address
these limitations

**USE AT YOUR OWN RISK**
