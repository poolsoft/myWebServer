# myWebServer
myWebServer library for esp8266/nodemcu arduino ide.  


I'm staring the library as an easy starting/base for working on the esp8266...  myWebServer will serve files from the SPIFFs on your device.  You should only use this on devices with available spiffs!  (4MB on nodemcu for example).

features:  

It will try and connect to your AcessPoint, if not config/connect it will auto-start local AP like "myespxxxx".  You just connect to that AP with your phone/tablet and it will display Wifi connect configuration.  (Uses captive DNS so you can just go to browser and type setup.com or "anything".com).  restart nodemcu after you've configured connection....

Afterwards once device connected to your local router/internet.  You go to it's local lan IP, or if your system supports mDNS you can type http://"device_name".local on your browser(device name is from setup from above).  

Virgin configs will bring up an integrated HTML file browser.  You can upload multiple files or drag files to top to allow you webserver to work...(index.html...etc).

supports OTA updating of ESP device via Wifi.

ntp time support will some methods to easily grab current date/time.

see sample htmls in folder for other features....

Library requires the use of the following libraries to be installed:

TimeLib for ntp here:  https://github.com/PaulStoffregen/Time
Arduino Json here:  https://github.com/bblanchon/ArduinoJson

this is still a WIP but I'll be updating as needed....I have other features I want to implement as well....



