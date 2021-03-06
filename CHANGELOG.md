# Change Log
All notable changes to this project will be documented in this file.

## Version 0.2.13
- Release date: April 26, 2018

### Fixed
- Fix board manager package version issue [#520](https://github.com/Microsoft/vscode-arduino/issues/520)

### Added
- Add install board command

### Changed
- Disable auto popup get started page for IoT Devkit

## Version 0.2.12
- Release date: April 8, 2018

### Fixed
- Fix board manager and library manager issue with portable Arduino installation [#415](https://github.com/Microsoft/vscode-arduino/issues/415)
- Fix board type button issue [#483](https://github.com/Microsoft/vscode-arduino/issues/483)
- Fix absolute output folder path issue [#450](https://github.com/Microsoft/vscode-arduino/issues/450)
- Fix serial port line ending issue [#497](https://github.com/Microsoft/vscode-arduino/issues/497)
- Fix debugging issue with file path contains spaces [#428](https://github.com/Microsoft/vscode-arduino/issues/428)
- Fix board manager mixed up packages issue [#414](https://github.com/Microsoft/vscode-arduino/issues/414)

Special thanks to [Felix Uhl](https://github.com/iFreilicht), [emontnemery](https://github.com/emontnemery), [tsalinger](https://github.com/tsalinger), [Diego Medeiros](https://github.com/Medeirox), [vphuoc](https://github.com/vphuoc), [Nuno Sousa](https://github.com/nuno407), thank you for your feedbacks.

## Version 0.2.11
- Release date: March 7, 2018

### Fixed
- Fix the issue caused by VSCode breaking change of `workspace.findfiles` [#467](https://github.com/Microsoft/vscode-arduino/pull/467)

Special thanks to [GarethE](https://github.com/keyoke), thank you for your contributions and feedbacks.

## Version 0.2.10
- Release date: October 27, 2017

### Changed
- Adopt the new VSCode Debug API [#432](https://github.com/Microsoft/vscode-arduino/pull/432), [#435](https://github.com/Microsoft/vscode-arduino/pull/435)
- Popup the example view when detecting new device is connected [#431](https://github.com/Microsoft/vscode-arduino/pull/431)

## Version 0.2.8
- Release date: October 10, 2017

### Changed
- Thanks to [Matthew Simms](https://github.com/brndmg) that fixes the regression from the usage react-select control in the [PR#421](https://github.com/Microsoft/vscode-arduino/pull/421)

## Version 0.2.7
- Release date: September 29, 2017

### Changed
- Default baud rate from 9600 to 115200

## Version 0.2.6
- Release date: September 1, 2017

### Added
- Add usb native binaries for electron 1.7.3 to unblock vscode insider August version

### Fixed
- Fix html/md preview issue

## Version 0.2.5
- Release date: August 24, 2017

### Added 
- Add settings for enabled/disable USB detection
- Add Arduino Example tree explorer viewlet
- Contribution from [DeqingSun](https://github.com/DeqingSun): Support multiple versions of Arduino on Mac [#375](https://github.com/Microsoft/vscode-arduino/pull/375)
- Contribution from [DeqingSun](https://github.com/DeqingSun): Add board support for STM32F1 with Arudino_STM32 [#377](https://github.com/Microsoft/vscode-arduino/pull/377)

### Changed 
- Leverage the ouput path config to speedup upload/verify
- Fix USB detection issue during uploading [#371](https://github.com/Microsoft/vscode-arduino/pull/371), [372](https://github.com/Microsoft/vscode-arduino/pull/372)
- Contribution from [lialosiu](https://github.com/lialosiu): Fix encoding issue for non UTF-8 [#364](https://github.com/Microsoft/vscode-arduino/pull/364)
- Update the documents with the helps of 
    - [eduherminio](https://github.com/Microsoft/vscode-arduino/pull/361)
    - [Atalanttore](https://github.com/Microsoft/vscode-arduino/pull/381), 

## Version 0.2.4
- Release date: July 3, 2017

### Added
- Add refresh button on boardmanager/librarymanager view to refresh index files manually

### Changed
- Update license and legal compliance fixes for open source
- The extension is ready for opening issue on github

## Version 0.2.3
- Release date: May 27, 2017

### Changed
- Use a new configuration page for switching arduino boards
- Lazy load the arduino extension on start up, only usb detection works in background, when it detects an arduino board, the extension will fully activate
- Update unit test to some basic arduino commands
- Fix some typos in code
- Fix issue #289 #324 #327

## Version 0.2.2
- Release date: May 19, 2017

### Added
- Support debug for a few boards: arduino zero/M0 Pro, AZ3166, Adafruit Feather M0, Adafruit WICED Feather
- Support debug for stlink, jlink

## Version 0.1.3
- Release date: May 12, 2017

### Added
- Support auto-discovery of AZ3166 board

### Changed
- Make activation condition to activate always for keeping USB auto-detection work background
- Auto-resolve arduino path from Registry on windows
- Well handle the case when vscode has no workspace

### Fixed
- Fix the issue of HTML view showing weird background color in vscode 1.12.1
- Fix arduino board installation failure on Mac after usb detection


## Version 0.1.2
- Release date: April 28, 2017

### Added
- Support manually imported library in libraries manager
- Support 3rd-party boards
- Add more devices (Arduino M0 Pro/Arduino Yún/Arduino Due) for auto discovery
- Add native binaries version for electron 1.6.6 to unblock VSCode's future upgrade
- Scaffold an empty sketch under current workspace folder

### Changed
- Make the arduino.json configurable through UI
- Refine extension activation events
- Restore previous active serial monitor after upload is completed
- Auto-resolve the sketch file path when the file is not existing for verify/upload
- Search custom libraries and examples in the path of sketchbook.path preference rather than default windows Document path

### Fixed
- Fix preferences.txt not found issue
- Fix verify command NPE issue when no serial port is selected
- Fix the error handling issue when opening serial monitor failed
- Avoid verify/upload reentry issue

## Version 0.1.1
- HotFix: Update display tag. 

## Version 0.1.0
- Release date: April 14, 2017
- Release status: Public Preview

### Added
- IntelliSense and syntax highlighting for Arduino sketches (based on [C/C++ for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools))
- Verify and upload your sketches in Visual Studio Code (based on [Arduino IDE](https://www.arduino.cc/en/main/software#download))
- Built-in board and library manager
- Built-in example list
- Built-in serial monitor
- Snippets for sketches
- Automatic Arduino project scaffolding
- Commond Palette (F1) integration of frequently used commands (e.g. Verify, Upload...)
