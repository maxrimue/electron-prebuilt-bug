This repo is thought to test whether people are affected by what seems to be a current bug in [electron-prebuilt](https://github.com/electron-userland/electron-prebuilt).

The mentioned bug causes Electron apps to not run animations under specific circumstances.
This example runs [Angular 1](https://angularjs.org) together with [Angular Material 1](https://material.angularjs.org/latest/), which is affected by this bug.

In order to test whether you are affected, follow these instructions:
  1. Clone this repository (`git clone https://github.com/maxrimue/electron-prebuilt-bug && cd electron-prebuilt-bug`)
  2. Install `electron-prebuilt` (`npm install`)
  3. Run `electron-prebuilt` (`npm start`)
  4. Click the visible blue button
  5. Close the dialog
  
If the dialog immediately opened and closed, you're probably not affected by this bug.
As it seems, following circumstances are required for this bug to show up:
  - Running the Electron App via `electron .` (with `electron-prebuilt` installed)
  - OS is OS X


[![Greenkeeper badge](https://badges.greenkeeper.io/maxrimue/electron-prebuilt-bug.svg)](https://greenkeeper.io/)