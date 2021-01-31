# Custom_Prusa_Mini
Instructions and pre-compiled firmware of the **prusa mini custom build** on thingiverse.

# Wiring of a 6-36V capacitive proximity sensor

From ![This answer by moderator](https://3dprinting.stackexchange.com/questions/6358/inductive-sensor-in-24-v-machine)

The inductive sensors work better when you apply a higher voltage than 5 V. Usually they are rated for 6-36 V, but please do check.
To prevent frying your board when connecting the sensor to (12 or) 24 Volts you could optically isolate the 5 V and the (12 or) 24 V circuit with an OptoCoupler module:

Image of an optocoupler module
![optocoupler module](https://i.stack.imgur.com/Xfrlg.jpg)

This module uses an optical switch based on the output of the sensor and should be correctly connected:

Image of connecting an optocoupler module to the sensor and to the board
![connecting an optocoupler module to the sensor and to the board](https://i.stack.imgur.com/munY6.jpg)

> Please note that the image uses a capacitive sensor rather than a inductive sensor, both are connected similarly wiring of an optocoupler module

Note that there are many sorts of sensors, a few are listed here. Generally speaking, the larger the diameter of the sensor, the larger the detection distance to the bed. Note that these work well with metal beds (Iron/steel better than Aluminium), but will not work for glass (capacitive sensors work on glass but are prone to drift by moisture in the air, a touch sensor may then be a better alternative).

# ESP3D v3.0 ALPHA for wireless printing & monitoring
Flash the pre-compiled esp3d_80e5de_alpha85.bin to your ESP32CAM and disconnect.Then waits for AP (ESP32CAM ..something like that) to show up.
After setting up the esp3d and connected to the interface, upload index.html.gz.

ESP3D v3.0 is able to print as host.No more limit on the file transfer stuff.
