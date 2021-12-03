# setup

1. login to unifi.ui.com
2. go to the Network application for the router
3. go to the LAN network in the settings and set the LAN CIDR to `10.101.8.1/16`
4. reboot all the access points.
5. reboot the router.


P.S. Step #3 knocks two access points offline :/. We will have to fix this. They are disabled for now.

# Fixed IPs

There is a DNS server setup at [http://dns.zephyr.network:9191/](http://dns.zephyr.network:9191/). The router needs to have fixed IPs for A records to keep working. To do this, we set a fixed IP for each virtual machine on zephyrnet so that we can keep DHCP for the office. Eventually I will have the router with a separate LAN with its own IP address management, but for now this we will manually keep DHCP reservations like this:

![image](https://user-images.githubusercontent.com/774794/144661383-1fd97338-322a-4fd2-a6aa-ec61aa9bed13.png)
![image](https://user-images.githubusercontent.com/774794/144661731-51b311be-9246-4395-82ef-f8383ed98c45.png)
