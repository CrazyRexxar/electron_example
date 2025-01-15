# Electron Create React Example

This is an example electron/create-react-app application, and serves as an example of how to structure your project if you want to share pieces of your codebase between electron and react.

Based on: https://medium.com/@johndyer24/building-a-production-electron-create-react-app-application-with-shared-code-using-electron-builder-c1f70f0e2649

Create-React-App building to binary for windows with electron and packaged with electron-builder.

## Build from source code by:
- Downloading Source Code or cloning repository
- Ensuring you have node JS v 18.16 or greater

## Install packages
### npm install

(commands for windows shown, also works on mac - see package.json for scripts)

## Check Installed Correctly
### npm run start-win

Then in a new cmd in the root dir
### npm run start-electron-win

## Build
### npm run build
### npm run build-electron-win

## If electron-build fails
Manually move /electron/main.js into the root of the /build folder

## Package
### npm run package-win
- Requires admin privileges to create .exe
- Requires developer mode to be ON to create sym.link for installer


## Project structure

- `electron/`: Code for the main Electron process
- `src/react/`: Code for the React renderer process
- `src/shared/`: Code shared between React and Electron
- `package.json`: Contains scripts for running the app in development, building it, and packaging it for production using electron-builder

