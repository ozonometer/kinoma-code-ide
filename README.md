This repo includes Kinoma Code IDE builds for Windows and Mac OS that I have built from Kinomajs source code. Sharing this as build for Windows is nowhere to be found on the internet. 
It was tested on Windows 10 and El Capitan. Windows version does not have simulators.
Since the Kinoma website is no longer available, there is no OTA update for device software, apparently, there is a way to create a bootable SD card for Kinoma Create with new software but I cannot find more information on that.
Kinoma Code IDE will fail to install apps on devices with old device software, it will fail with "Break: require: invalid script!", because of this I reverse-engineered Kinomablocks communication with Kioma Create and created a Java 11 program that installs apps on outdated devices, the downside is that only works for JavaScript files, no images or other files.
To use it it requires Java 11 runtime or SDK. To install the app, save the app script in the main.js file, open the Java program (see attached images) and enter the device IP, app name, and path to the folder where main.js is saved, click Install.

Windows 10 Screenshot:
![image](https://github.com/ozonometer/kinoma-code-ide/assets/15060227/083bd170-4f53-4183-8b67-a42edb90238c)

El Capitan Screenshot:
![Screen Shot mac](https://github.com/ozonometer/kinoma-code-ide/assets/15060227/2a9a58de-0c70-43d3-a5a3-fa770c6a694e)


Java 11 program to install scripts
![image](https://github.com/ozonometer/kinoma-code-ide/assets/15060227/1279ddd1-4365-4594-9178-aa8a4f2d18cf)
![image](https://github.com/ozonometer/kinoma-code-ide/assets/15060227/93108ee2-5da2-4017-adce-99cf008ff639)

