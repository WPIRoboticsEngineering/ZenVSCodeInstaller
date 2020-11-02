# ZenVSCodeInstaller
Instructions and Installer scripts for VSCode configured for use in the WPI robotics program

# Setup Instructions

## 1 install VSCode+Platformio

Find the installer for VSCode here:

https://code.visualstudio.com/

## 2 Open VSCode and Install PlatformIO

Open VSCode Extension Manager

<img src="image/openExtMng.png" width="600">

Search for official `PlatformIO IDE` extension

<img src="image/searchPio.png" width="600">

Install `PlatformIO IDE`

Close VSCode to complete setup

## 3 Download the example code

[Source Code Zip for Latest RBE1001Lib](https://github.com/WPIRoboticsEngineering/RBE1001Lib/archive/0.10.0.zip)


Open the folder where you download the examples


<img src="image/showInFOlder.png" width="600">

Select Extract All


<img src="image/extractall.png" width="600">

Extract to a known location, we recommend Documents\RBE1001Lib


## 4 Open an Example

Open VSCode and select the new PlatformIO Plugin Icon

<img src="image/selectPIOHome.png" width="600">


Select Import Arduino Project

<img src="image/importArduino.png" width="600">

For the Board field set

`Espressif ESP32Dev Module`

And Navigate to the folder you used to extract the RBE1001Lib directory in Step 2


<img src="image/esp32Board.png" width="600">

Navigate into the `examples` folder and select one, in this case `FullSystemTest`

Select Import

<img src="image/import.png" width="600">


The first time you do this it will take a long time as PlatformIO needs to download and install the ESP32 toolchain.

## Configure the projects libraries

Open the file `platformio.ini` in your new project and make the entire contents of the file read:

```
; PlatformIO Project Configuration File
;
;   Build options: build flags, source filter
;   Upload options: custom upload port, speed and extra flags
;   Library options: dependencies, extra library storages
;   Advanced options: extra scripting
;
; Please visit documentation for the other options and examples
; https://docs.platformio.org/page/projectconf.html

[env:esp32dev]
platform = espressif32
board = esp32dev
framework = arduino
monitor_speed = 115200
lib_deps =
  ESP32AnalogRead
  ESP32Encoder
  Esp32WifiManager
  ESP32Servo
  ;RBE1001Lib @ 0.9.4  ;Shim V3
  RBE1001Lib @ 0.10.0  ;Shim V2
  WebServer

```

### V2 Shim Red Board

If you have the V2 shim, use the code above. 

### V3 Shim Red Board

If you have the V3 shim, uncomment the line switching the library version to 0.9.4 and comment out the line for 0.10.0

