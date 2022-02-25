This document covers the generation of the BCM20702A0-0489-e031.hcd file
to bring the Fujitsu Celsius H910 bluetooth chip to work under Linux Mint 20.3

First I compiled the executable file hex2hcd from the hex2hcd.c
This was done by just typing
make
within the hex2hcd-master/ directory.

then I generated the wanted BCM20702A0-0489-e031.hcd file by performing the operation
mypc:~$ ./hex2hcd BCM20702A0_001.001.024.0156.0204.hex BCM20702A0-0489-e031.hcd

I copied the BCM20702A0_001.001.024.0156.0204.hex file from a working Fujitsu Celsius H910
Windows 10 Installation to the hex2hdc-master directory.

Then I generated the wanted BCM20702A0-0489-e031.hcd file by performing the operation
my@fujitsu-h910:~$ ./hex2hcd BCM20702A0_001.001.024.0156.0204.hex BCM20702A0-0489-e031.hcd

At last I copied the generated BCM20702A0-0489-e031.hcd file to the /lib/firmware/brcm/
I rebooted my Fujitsu H910 Laptop and could finaly connect to al my bluetooth devices.

I hope, this can help to solve your problems!

Hans
