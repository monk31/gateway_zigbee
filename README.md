# gateway_zigbee
gateway zigbee raspberry JN5169


If you want to control a smart plug , or light a lamp or monitoring temperature with your smartphone
this application can help you

I use a raspberry pi 3 to make a gateway zigbee but you can also use a beaglebone black with ethernet link.

To communicate with my zigbee device, I choose a excellent application on my mobile phone : "IOT on off", you can download with applestore or playstore
see this link : https://www.iot-onoff.com/ for more details

this project has build with three binary and one script in python

see Wiki for installation with a raspberry pi3

you can download "Net Analyser" to scan your network at home
you must configure broker adress to set your smartphone

Three kinds of device can be appairing in the zigbee network :
xiaomi smart plug
xiaomi device sensor temperature
lamp hue

![IMG_1367](https://user-images.githubusercontent.com/13630510/63885449-acc19f00-c9d8-11e9-9ec0-f208ed234d65.png)


# Appairing Device

to appair device in the network

use the topic "cmd/join" with payload ="23", after you are 180 s to appair the device

for the smart plug , press 5 s on the button







I do a summary of topic that you can configure with your smartphone

 topic state  -> "/sensor/state" + id device  : to know the feedback state of your smart plus or lamp

 topic tmemperature -> "sensor/tmp" + id device
 
 topic humidity -> "sensor/hum" + id device
 



