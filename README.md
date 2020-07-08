# Set up dell_c1760nw printer on Ubuntu 20.04

## Printer Model
dell_c1760nw is a wrapper of Xerox-phaser-6000B

## GUI Settings  
In Settings --> Printers --> Add..  
Select 'dell_c1760nw' which is in your local network.  
Add driver, select recommended model 'Xerox-phaser-6000B', because dell_c1760nw is not in the driver list.  

## Command line
sudo apt-get install lib32z1  
sudo apt-get install libcupsimage2:i386

You may also need do:  
sudo chmod 755 -R /usr/lib/cups/filter  
sudo chown -R root /usr/lib/cups/filter

The printer should work now. That's it!

