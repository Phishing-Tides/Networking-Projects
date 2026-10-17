Equipment used:
1. Four Desktops
2. 1 Switch
3. 1 Router
4. Meraki Device
5. 2-3 Cell Phones

How I did it:
I started by creating a small environment and connected every device to the network switch. After connecting the wires, I fired up the CLI for the router and set up a network.

I then created a DHCP Pool that I just called "LAN_POOL". I set up the range for 192.168.1.0 to 255.255.255.0, default router to 192.168.10.1 (A Mistake I made that I fixed later). I also set the DNS Server to google(8.8.8.8).

I then opened one of the PC's and tried to switch the IP configuration from static to DHCP. I kept getting a "DHCP Failed" error message and then realized that the router's IP was set to 192.168.1.1 and not 192.168.10.1. I then fixed my mistake by removing the old DHCP configuration and making the new one with the correct IP Address.  
