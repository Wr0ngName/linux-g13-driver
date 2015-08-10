# linux-g13-driver

I needed a way to get my Logitech G13 up and running fast, and I found this one.
I am running Linux Mint 17 x64. After a few teaking, it is running as expected,
and provides a quick workaround to the original drivers.

The drivers are no longer maintained by the original projects, I do not especially
intend to continue, as it is still working properly after a few work.

## Requirements
libusb-1.0
if you don't have it, you can get it by "sudo apt-get install libusb-1.0"

Java version 1.6 or higher

## Download
Download zip file from http://code.google.com/p/linux-g13-driver/downloads/list
Unzip into your favorite directory

## Build
Open a console (command prompt)
Go to the directory where you unzipped your download
type "make"

## Running Application
Run the config tool first!
In a command prompt go to the directory where you unzipped your downloadand type "java -jar Linux-G13-GUI.jar"
This will bring up the UI and create the initial files needed for your driver.
All config files are saved in $(HOME)/.g13

##Run the driver
In a command prompt go to the directory where you unzipped your download and type "sudo ./G13-Linux-Driver"

If you are configuring the application while the driver is running, the driver will
not pick up changes unless you select a different bindings set or you can restart
the driver.

The top 4 buttons under the LCD screen select the bindings.

The joystick currently only supports key mappings.

Thanks to Jim Gupta for the code (https://code.google.com/p/linux-g13-driver).
