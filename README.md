IMPOERTANT NOTE! This file has been incorporated into the JackTrip Virtual Device
software, so there is no longer any need to manually incorporate it yourself.

This file is to make your Raspberry Pi running the JackTrip disk image from the
JackTrip Foundation accept most USB connected audio adapters, interfaces, or mixers.
The jacktrip-init.sh file in this repository replaces the file of the same name
in the directory /usr/local/bin/ on the Raspberry Pi.

In order to replace this file, you will need to:
* Copy jacktrip-init.sh from this repository to your computer
* Open two terminal windows on your computer (where you have placed the new file)
* In first window, "ssh" onto your Raspberry Pi (see document below)
* Use the "rw" command to make the filesystem writable
* In second window, transfer the new file using "scp" onto your Raspberry Pi
* That will leave the file in /home/pi
* In the first window, "cd" to /usr/local/bin
* (optional but recommended just in case) Save a copy of jacktrip-init.sh
* Move the file in ~/jacktrip-init.sh to the current directory (use "sudo mv")
* Use the "ro" command to make the filesystem readonly
* Reboot your Raspberry Pi

Helpful links:

Document on how and why to use this jacktrip-init.sh file
https://docs.google.com/document/d/1jtnWEsLEt3lfJjqtlQriXOR7B5rb0PyMrvU51t1I2AI/edit

Instructions on how to ssh onto the Raspberry Pi running the Virtual Studio Image
https://jacktrip.zendesk.com/hc/en-us/articles/360058876413-Troubleshooting-the-Virtual-Studio-Image

Virtual Studio Image for Raspberry Pi
https://jacktrip.zendesk.com/hc/en-us/articles/360055205313-Virtual-Studio-Image-for-Raspberry-Pi
