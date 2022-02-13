# L515-WIth-Jetson-Nano
L515 Jetson Nano

You can refer the article linked here https://github.com/IntelRealSense/librealsense/blob/master/doc/installation_jetson.md to do custon installation, or you could do the following steps mentioned below (refred frm jetsonhacks.com)

Open the terminal on ypour jetson nano and put the following commands.
1)
$ git clone https://github.com/JetsonHacksNano/installLibrealsense

2)
$ cd installLibrealsense

3)
$ ./installLibrealsense.sh

4)
To start the realsense Viewer
$ realsense-viewer


So we have completed the software side here. Now to connect the L515 liDAR Camera with jetson nano we need to give it more power and start it in Max power mode(That is 5v 4A, connected via barrel jack or usb c), or else the jetson Nano would power off. follow the below steps if you havent already configured it.

1. Turn off the Jetson Nano and disconnect everything connected to it.
2. use a jumper and connect it to pin x and y
3. now connect the power adapter on the barel jack port
4. start the nano and on the dextop navigate to power setting
5. and click on power mode and set it to "Maxn"




