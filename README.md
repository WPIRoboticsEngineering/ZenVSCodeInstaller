# Installing VSCode/platformio

Instructions and Installer scripts for VSCode configured for use in the WPI robotics program

# Setup Instructions

## 1) install VSCodium <= 1.45.1

The VSCodium project exists so that you don’t have to download+build from source. This project includes special build scripts that clone Microsoft’s vscode repo, run the build commands, and upload the resulting binaries for you to GitHub releases. These binaries are licensed under the MIT license. Telemetry is disabled.

[Windows](https://github.com/WPIRoboticsEngineering/ZenVSCodeInstaller/releases/download/0.0.0/VSCodiumSetup-x64-1.45.1.exe)

[MacOS](https://github.com/WPIRoboticsEngineering/ZenVSCodeInstaller/releases/download/0.0.0/VSCodium.1.45.1.dmg)

[Ubuntu](https://github.com/WPIRoboticsEngineering/ZenVSCodeInstaller/releases/download/0.0.0/codium_1.45.1-1589539594_amd64.deb)

[Other](https://github.com/VSCodium/vscodium/releases/tag/1.45.1)


### 1.1) MacOS users ONLY

Install the Developer Command Line Tools from Apple (this is the thing that is currently broken). To do it you need to go to [developer.apple.com](https://developer.apple.com) and create an account. This is all pretty annoying, but it gets around the problem. Then navigate to the [download page for the tools](https://developer.apple.com/download/more). Check the boxes as shown on the sidebar (“Developer Tools” and “macOS”) as shown in the screen image above. Then download “Command Line Tools for Xcode 12”. It’s a pretty hefty download, but it should make everything work. After you download the tools, double click on the file in your Downloads folder to install.

<img src="image/osxXcode.png" width="300">

Now you can run VSCode by hitting Command-Space, type in “visual studio Code”. 

### 1.2) Read about why we use VSCodium instead of VSCode

[We are protecting your private data.](usevscode.md)


## 2) Open VSCode and Install PlatformIO

Open VSCode Extension Manager

<img src="image/openExtMng.png" width="600">

Search for official `PlatformIO IDE` extension

<img src="image/searchPio.png" width="600">

Install `PlatformIO IDE`

Close VSCode to complete setup

## 3) Open Your Starter Code

### 3.1) **Pro/Con of Example Code**

Choose this option while *building/testing* your robot

#### Pro

 * Quickly Open Examples
 * Quickly Test Hardware
 * Lots of different examples
 * Best for running code you don't intend to change
 
 
#### Con 

 * Difficult to collaborate with team
 * Difficult to share code with staff for online help
 * Impossible  to go back in time to a previous version  
 * Possible to lose all of the code 
 * Awkward to go download the source and open it (This is a VSCode limitation)
 * Difficult to find additional examples for other libraries (This is a VSCode limitation)
 
### 3.2) **Pro/Con of Git**

Choose this option while *programming* your robot

#### Pro

 * Project is pre-configured, no need to mess with the platform.ini or .gitignore
 * Easy to collaborate with team
 * Easy to share code with staff for online help
 * Version history of every committed change, you can always go back in time
 * Code backed up on a server and accessible to whole team
 * GitHub Desktop helps make the Git workflow understandable and merge conflicts easier to resolve
 * Best as the starter code for the Final Project
 
#### Con

 * Only the one example in the Template, the RCCTL example 
 * Git is one more thing to learn, although utterly essential long term, not required for 1001
 * Collaboration with teams means the possibility of merge conflicts/resolutions

### 3.3) Choose

either

[Follow these instructions for Examples as starter code](openExample.md)

or

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


