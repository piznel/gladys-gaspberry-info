# Gladys-Raspberry-Info

A module that turns possible getting information from Raspberry, such as GPU/CPU temperature, serial number, IP, etc. since Gladys.
<div align="center">
<img src="https://user-images.githubusercontent.com/25089531/51909914-08d62d80-23ce-11e9-9bfb-b1003a866393.png" width="500" />
</div>

1. Add this module to Gladys:

   * Name: `Gladys-Raspberry`
   * Version: `0.1.0`
   * URL: `https://github.com/piznel/gladys-raspberry-info.git`
   * Slug = `rpi-info`

2. Restart Gladys.

3. 3 devices have been created, allowing to follow:

     * CPU temperature
     * GPU temperature
     * CPU voltage

In the "Module Configuration" page, you will also find information about your Raspberry, as well as statistics such as "memory" and "network". You will also find 3 tabs:

* In the "**Hardware**" tab, a button allows you to display the list of USB devices, as well as the address of the serial port used:
<img src="https://user-images.githubusercontent.com/25089531/51909981-302cfa80-23ce-11e9-99d4-a1363fe44f40.png" width="500" />

* In the "**Software**" tab, you will find a "Bash Command" button, allowing you to enter bash commands, as in the console, and the result will be returned to you. For example :

  * `lsusb` : gives the list of devices connected in USB.
  * `lsusb -v | grep -Ei '(idVendor)'` : List all devices in your system (only vendor name).
  * `lsusb -t`: Find USB device supported speeds by using tree structure option.
  * `ifconfig` : To check which network the wireless adapter is using.
  * `iwlist wlan0 scan` : Prints a list of the currently available wireless networks "wlan0".
  * `cat /proc/partitions` : reveals the size and number of partitions on your SD card or HDD.
  * `nmap -sP 192.168.0.*`: check which hosts are live and up in Network "192.168.0.*"
  <img src="https://user-images.githubusercontent.com/25089531/51910065-65394d00-23ce-11e9-93af-16827bab097e.png" width="500" />

* In the "**Security**" tab, you will find a list of current connections to your rapsberry, as well as a button displaying the list of the last 5 connections and their status.

4. The monitoring box

An additional box has been added in Gladys. Test it!

<div align="center">
  <img src="https://user-images.githubusercontent.com/25089531/51909724-95ccb700-23cd-11e9-94c2-5ba2fd4ff9cd.png" width="500" />
</div>
