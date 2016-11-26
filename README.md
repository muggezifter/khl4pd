# README #

pd patches for the khl4 project

####instrument 1
khl4a.pd
khl4b.pd

To make the pi use the external sound card by default:

1. Disable analog audio:
  * Open `/boot/config.txt` and comment out `dtparam=audio=on`.
2. Set the USB audio device to the default device:
  * Open `/lib/modprobe.d/aliases.conf` and comment out the line options `snd-usb-audio index=-2`
3. Reboot

see [here](http://superuser.com/questions/989385/alsa-base-conf-missing-in-new-raspberry-pi-raspbian-jesse)
