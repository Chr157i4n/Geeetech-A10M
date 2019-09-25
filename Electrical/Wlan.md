I tested three methods for adding Wlan to my printer:

1. Octoprint

https://octoprint.org/

You can either install Octoprint on a running raspberry pi, or install octopi as an operation system on a pi.
Octoprint can be connectet to your wireless network and offers a webinterface.
The printer can be connected to an USB port of the pi. A display is not needed.

Octoprint offers a lot of functions, but on the other hand it can control only one printer at a time.
Also the G-Code is stored on the PI and therefore the upload is fast, but the PI send command after command to the printer and 
if the PI crashes or loses power, the printer will stop printing.

2. Geeetech 3DWifi

https://www.geeetech.com/wiki/index.php/3D_wifi_module

Geeetech offers a wifi_module for 3D printers. It is based on an ESP8266 chipset and has and USB-port for the power and one USB-port for the printer.
The disadvantage of this product is, that is has no webinterface and can only be used with a smartphone app.

3. ESP3D

https://github.com/luc-github/ESP3D

The SKR-PRO 1.1. offers a slot for an ESP01s board. with Pins for the powering and a serial connection to the ESP.
For this ESP there is the open source firmware ESP3D.
It offers a Webinterface with all necessary function.
If you upload a G-Code file to the printer, the ESP will store it on SD card of the printer. That is slower, 
but you have the advantage, that even if you start the print from the webinterface, the printer will continue to print, even without the ESP.

