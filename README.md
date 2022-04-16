# L515-WIth-Jetson-Nano


## A) First we will setup our Jetson Nano (You can skip this if you have installed jetpack)

Refer the following link for installing Jetpack on Jetson Nano https://developer.nvidia.com/embedded/learn/get-started-jetson-nano-devkit#intro


## B) Now we need to install Intel Realsense on Jetson nano, you can refer the article linked here https://github.com/IntelRealSense/librealsense/blob/master/doc/installation_jetson.md to do custon installation, or you could follow the steps mentioned below.

Open the terminal on ypour jetson nano and put the following commands.


1)
$ git clone https://github.com/JetsonHacksNano/installLibrealsense


2)
$ cd installLibrealsense


3)
$ ./installLibrealsense.sh


To start the realsense Viewer

4)
$ realsense-viewer


## C) So we have completed the software side here. Now to connect the L515 liDAR Camera with jetson nano we need to set it to Max power mode(That is 5v 4A, connected via barrel jack or usb c), or else the jetson Nano would power off as the L515 requires more power. Follow the steps givenbelow if you havent already configured it to Max power mode.

1. Turn off the Jetson Nano and disconnect everything connected to it.
2. Use a jumper and connect it to pin J48
3. Now connect the power adapter on the barel jack port
4. Start the nano and on the dextop navigate to power setting
5. Click on power mode and set it to "Maxn"

## d) Now connect L515 to Jetson Nano and start the realsense viewer by using the command  

$ realsense-viewer 


