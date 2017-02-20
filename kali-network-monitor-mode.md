# Kali Network Monitor Mode

`ifconfig wlan0 down` - turn off the adapter

`iwconfig mode monitor` - turn on monitor mode setting

`ifconfig wlan0 up` - turn on the adapter

After this is done, connect to network as normal.

Now your network card will capture ALL packets it can see and not only the ones that pertain to it. 
