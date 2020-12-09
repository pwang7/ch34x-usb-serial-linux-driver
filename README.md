# Linux Driver for USB Serial Chip ch34x

The steps to build and install the driver:
* Build the driver: `make`
* Remove the old driver: `sudo mv /lib/modules/$(uname -r)/kernel/drivers/usb/serial/ch341.ko .`
* Install the new driver: `sudo cp ch34x.ko /lib/modules/$(uname -r)/kernel/drivers/usb/serial/`
* Update module dependency: `sudo depmod`
