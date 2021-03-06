buttonOSC
=========

Send button presses over OSC to and from 2 pd patches, activating an LED and a solenoid.

This is intended for having the same setup on 2 devices on the same network.
Once a network has been established between the 2, get the ip addresses. 

Get the [[pduino]](http://puredata.info/downloads/pduino) object and put it in the same folder as buttonOSC.pd

Use this schematic to connect the solenoid to pin 2.
http://www.instructables.com/id/Controlling-solenoids-with-arduino/

Connect an LED to pin 6.

Connect a button to pin 9.

Make sure to substitute "localhost" with the destination device's ip address.
![ipaddress](https://epicjefferson.files.wordpress.com/2014/10/ip.png)

Make sure to set [dumpOSC] to listen to the port being transmitted by the opposite device.
![dumpOSC](https://epicjefferson.files.wordpress.com/2014/10/dumposc.png)

Here's an example of how OSC needs to be setup.
![OSCprotocol](https://docs.google.com/drawings/d/1wAG7VVWRZLQ_Gt673qnJcaQuxo04y9ZNKDu_ImknVbY/pub?w=916&amp;h=380)