# blheli-configurator

Google Chrome application for BLHeli firmware flashing and configuration.

[![available in the Chrome web store](https://developer.chrome.com/webstore/images/ChromeWebStore_Badge_v2_206x58.png)](https://chrome.google.com/webstore/detail/blheli-configurator/mejfjggmbnocnfibbibmoogocnjbcjnk)

## Disclaimer

This software is provided as is, use it at your own risk. **ALWAYS REMOVE THE PROPELLERS** and power your ESCs via a **current-limiting** device or power supply.

## Features

* Only BLHeli passthrough supported at the moment, hence only **CleanFlight**,  **BetaFlight**, **INAV** and **TriFlight**
* Changing settings for any BLHeli_S, BLHeli SiLabs and BLHeli Atmel ESCs with bootloader
* Flashing BLHeli and BLHeli_S to SiLabs and Atmel ESCs

## Future plans

* Add declarative UI description for MAIN and MULTI modes
* Full-featured 4-way interface support via BLHeli boxes, with C2-interface support
* Electron/NW.js wrapper with auto-update
* Android/iOS version based on the same code-base

## Adding a new BLHeli revision or new supported ESC

You can submit pull requests to js/blheli_versions.json and js/blheli_escs.json files, user installations of BLHeli Configurator will see the changes shortly.

## Building

This project uses ReactJS, JSX and some modern ECMAScript extensions and depends on `npm` for building.
Following the initial checkout, you have to run:
```
npm install
```
After that, to actually compile all the required .jsx files, run:
```
npm run build
```

## Usage

Having enabled Developer Mode in Chrome, navigate to chrome://extensions/ and use **Load unpacked extension...**, providing path to the root directory of your working copy.

Launch the application, plug your flight controller into a USB port, press **Connect**, power your ESCs.
If you run into problems while working with the program, make sure to copy Developer's Console output as well as save log using the **Save Log** button.

## Thanks

This software started as a tab in [Cleanflight Configurator](https://github.com/cleanflight/cleanflight-configurator), hence my deep appreciation to all of you who contributed to it's development.

Special thanks to everyone who helped me with development, testing, collecting of logs and ideas and all other stuff:
* *Stefan van der Ende*
* *Nathan*
* *Steffen Windoffer*
* *Steven R. Lilly*
* *Tuomas Kuosmanen*
* *Robyn Bachofer*
* *ByeJon* from the IntoFPV forum for drawing an icon :-)

This list is extended as the development goes on and I remember all the names :)
