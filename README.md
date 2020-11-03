# Installing VSCode/platformio

Instructions and Installer scripts for VSCode configured for use in the WPI robotics program

# Setup Instructions

## 1) install VSCode

Find the installer for VSCode here:

https://code.visualstudio.com/

### 1.1) MacOS users ONLY

Install the Developer Command Line Tools from Apple (this is the thing that is currently broken). To do it you need to go to [developer.apple.com](https://developer.apple.com) and create an account. This is all pretty annoying, but it gets around the problem. Then navigate to the [download page for the tools](https://developer.apple.com/download/more). Check the boxes as shown on the sidebar (“Developer Tools” and “macOS”) as shown in the screen image above. Then download “Command Line Tools for Xcode 12”. It’s a pretty hefty download, but it should make everything work. After you download the tools, double click on the file in your Downloads folder to install.

<img src="image/osxXcode.png" width="300">

Now you can run VSCode by hitting Command-Space, type in “visual studio Code”. 


## 2) Open VSCode and Install PlatformIO

Open VSCode Extension Manager

<img src="image/openExtMng.png" width="600">

Search for official `PlatformIO IDE` extension

<img src="image/searchPio.png" width="600">

Install `PlatformIO IDE`

Close VSCode to complete setup

## 3) Open Your Starter Code

[Follow these instructions for Example Programs](openExample.md)

[Follow these instructions for Git with a Template Repo of starter code](useGit.md)

## 4) Compile

Hit the compile (the little check mark) and verify that the example completes with `SUCCESS`

<img src="image/compile2.png" width="600">

## 5) Upload code to ESP32

Hit the upload button (the little right arrow) and verify it completes with success

<img src="image/upload.png" width="600">

### 5.1) If you get anything other than success, install the driver for you system

[Esp32 Driver Windows](https://github.com/WPIRoboticsEngineering/ESP32ArduinoEclipseInstaller/releases/download/0.0.0/CP210x_Universal_Windows_Driver.zip)

[Esp32 Driver MacOS](https://github.com/WPIRoboticsEngineering/ESP32ArduinoEclipseInstaller/releases/download/0.0.0/SiLabsUSBDriverDisk.dmg)


