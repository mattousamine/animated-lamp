## rtl8188eus v5.3.9

# Realtek rtl8188eus &amp; rtl8188eu &amp; rtl8188etv WiFi driver
Copyright to: https://github.com/kimocoder

TESTED ON KALI LINUX 2019.
# HowTo build/install commands (use root mode or write sudo before commands)
1) apt update && apt upgrade 
2) apt install -y bc linux-headers-am64
3) git clone https://github.com/mattousamine/animated-lamp.git
4) cd animated-lamp
5) cp realtek_blacklist.conf /etc/modprobe.d
6) make
7) make install

# MONITOR MODE howto (you need to do this after every reboot)
Use these steps to enter monitor mode.
1) systemctl stop NetworkManager.service (to make it back to the managed mode put: service network-manager start)
2) iwconfig wlan0 mode monitor

DONE !!!



