# Benq-projector-remote-script

RS232 benq projector remote control under Linux

<i>Goal is to power on and power off the projector automagically when the computer is turned on and off</i>


<b> Hardware setup :</b>

USB to RS232 serial converter (Trendnet TU-S9)

RS232 null modem cable

Benq MX620ST


<b>Software setup :</b>

Linux mint 17.1


<b>Useful links :</b>

BenQ RS232 Commands : http://www.benq.com/download/projector/SW916/RS232%20command/BenQ%20RS232%20Commands.pdf

Linux serial permissions : http://websistent.com/fix-serial-port-permission-denied-errors-linux/

as root, copy benqremote in /etc/init.d
make it executable
chmod +x /etc/init.d/benqremote

Apply service permissions for script to be executed in the right runlevels

update-rc.d benqremote start 30 2 3 4 5 . stop 70 0 1 .

Ultra big up to my linux heroes : 
Brice https://github.com/tmator
& Fabrice https://github.com/sack
