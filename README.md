# EasEE As Pi

A simple setup and boot script to make the Pi's GPIO pins more accessible. Even for experienced programmers it should make the time needed to setup a Pi for GPIO control much faster.

For pinouts goto http://pi.gadgetoid.com/pinout though I included pictures for reference too

Note that everything is handled by the settings which the program looks for in the boot directory. 

## Script Installation

boot the Pi and run the install script (install.sh) 
make sure the patch file is at the same level as the install script
make sure to place EasEEPi.py in the boot folder and a settings XML file to read from

You have to make your own settings file though there is Gooey-Pi for a easy visual setup.

## Manual Installation

to get this to run at boot create a folder named audio on the boot partition and put piDAR.py and settings.xml in the boot folder. Then edit rc.local which is found in /etc/ by doing

    sudo nano /etc/rc.local
	
and then replace the IP dummy script with

    sudo python /boot/EasEEPi.py

Make sure to edit the settings file to the layout you would like
   
   
## To Do:
+ more customizable output control
