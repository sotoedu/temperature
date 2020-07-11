https://www.circuitbasics.com/raspberry-pi-ds18b20-temperature-sensor-tutorial/

$ sudo nano /boot/config.txt

dtoverlay=w1–gpio

$ sudo reboot

$ sudo modprobe w1–gpio

$ sudo modprobe w1-therm

$ ls /sys/bus/w1/devices 

28-000006637696 w1_bus_master1 is displayed in my case.

$ python namds18b20.py

vcc and data is linked register
sensor   ||   board pin (Not GPIO)
vcc      =   1 (3.3v)
gnd      =   6  
data     =   7 (GPIO4)
