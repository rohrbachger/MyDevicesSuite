# MyBootMedium One blade from admins swiss knife
This is a HowTo for creating Windows PE images booting from CD/USB/PXE.
It is not too public, that the WIM format, a standard Windows can be used very easy to make backups and installations.
There are a lots of tools available to create bootable ISO or USB like PE Builder. You can add nearly every app like browser and several other tools, they have nice frontends and are heavy loaed with functionality.
My basic needs are simple, so I added only SSH and UltraVNC. This allows to reach the PXE booted machine from remote.

The goal of this project is, to show how a simple PE image 32/64 bit can created. Easyly you can add your own background and
own extensions.
Like it is very common you can burn a CD or create a usb boot stick, but with iPXE, a special PXE boot, you can boot over the network. As iPXE uses http, the boot is much faster than over the normal PXE tftp. Also iPXE allows nice boot menues, and e.g. it is possible to create MAC address based configurations. PE images with 500MB boot in less than 1 minute.
As you need some environment for the PXE / iPXE boot this is more for company usage then for private use:

Needs:
DHCP server with posibilty to set Options ( Windows DHCP / Linux DHCP)
tfpd service on one machine in the network.
http service somewhere reachable.

Linux machine like Ubuntu to create/build once the special undionly.kpxe file.

Download the WAIK Kit for Windows 8.1 or Windows 10.
Clone this project

