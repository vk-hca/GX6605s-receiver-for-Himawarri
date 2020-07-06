# GX6605s-receiver-for-Himawarri
Create a dvb-s2 tcp reciever from a low cost set top receiver with the C-sky provided linux kernel and tools

This project relies on learning to contol the demodulator used if it proves to be able to demod the stream, then develop a new flash for the receiver or a plug in to add to the factory code.

This receiver is rather unusual, in the that:

- The manufacturer of the chipset provides a maintained linux kernel and buildroot tool chain for it with Qemu support on Git hub complete with demo code for serial, video players etc.

- There is a development board readily available for the GX6605s chip with jtag, hdmi and usb etc.

-  The chip set is widely used in receivers sold around the world by different bands names and readily available and offers an alternative development platform.

- With a usb wifi adapter telnet with putty as root allows full access.

- The well known " Busybox" provides system functionality.

- There is a more advanced version gx6622 chip used in receivers with a serial port and wired ethernet.

- The receiver software uses kernel modules loaded at boot to configure an control the tuner, panel, etc, after boot the main code can be killed off.

- Any usb stick inserted is mounted at /media/sda1 and is completely accessible.

- Untested but the receiver will boot from usb.

- An external bios is stored in spi eeprom making it hard to brick the box.

There is not a great amount of processor speed and system resources but its an inexpensive device.

For the provided linux code and tools look here:

https://github.com/c-sky

These links give info on the development board:

 https://c-sky.github.io/docs/gx6605s.html


https://www.mickmake.com/post/csky-s...he-sky-review/

https://www.cnx-software.com/2018/11...05s-media-soc/

http://feeds.feedburner.com/co/NGpS

https://www.arb-softwares.com/2019/0...tech-2019.html

Specs for the development board.

CPU CSky
CPU Frequency 600 MHz
Chipset GX3211
Board GX6622-dvbs2
RAM 128 MB
RAM Frequency 533 MHz
ROM Type MX25L64
ROM Size 8 MB



