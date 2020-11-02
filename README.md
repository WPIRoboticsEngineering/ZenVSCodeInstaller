# ZenVSCodeInstaller
Instructions and Installer scripts for VSCode configured for use in the WPI robotics program

# Setup Instructions

## 1 install VSCode+Platformio

Find the installer for VSCode here:

https://code.visualstudio.com/

## 2 Open VSCode and Install PlatformIO

Open VSCode Extension Manager

<img src="image/openExtMng.png" width="300">

Search for official `PlatformIO IDE` extension

<img src="image/searchPio.png" width="300">

Install `PlatformIO IDE`

Close VSCode to complete setup

## 3 Download the example code

[Source Code Zip for Latest RBE1001Lib](https://github.com/WPIRoboticsEngineering/RBE1001Lib/archive/0.10.0.zip)


Open the folder where you download the examples


<img src="image/showInFOlder.png" width="300">

Select Extract All


<img src="image/extractall.png" width="300">

Extract to a known location, we recommend Documents\RBE1001Lib


## 4 Open an Example

Open VSCode and select the new PlatformIO Plugin Icon

<img src="image/selectPIOHome.png" width="300">


Select Import Arduino Project

<img src="image/importArduino.png" width="300">

For the Board field set

`Espressif ESP32Dev Module`

And Navigate to the folder you used to extract the RBE1001Lib directory in Step 2


<img src="image/esp32Board.png" width="300">

Navigate into the `examples` folder and select one, in this case `FullSystemTest`

Select Import

<img src="image/import.png" width="300">



