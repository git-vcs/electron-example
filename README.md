# electron-packager-example

This is an electron example that builds installers for different machine architecture and opperations system with the help of the community made  [Electron-builder](https://github.com/electron-userland/electron-builder)

This example builds for:
Windows(32 bit and 64 bit)
Linux(32 bit, 64 bit and armv7) 
MacOS(64 bit)

## How to build:
To make all the possible version write: npm run-script buildIntallers
This builds the installers defined in the build section in package.json
However depending on your OS you may need to install extra dependencies.

## To specify the OS and architecture to build for: 
1. install Electron-builder globally: npm install -g electron-builder
	  
2. then type: electron-builder --linux deb --x64
				    
This make installer for linux diustrobutions with the .deb pakcage running 64-bit architecture.
For the full list of possible configurations see [Electron-builders website](https://www.electron.build/)


### note: 
only the Linux installers(armv7l) is tested.


# Todo:
Make pipeline for generating all possible installers on github-actions.
Sign windows executable. 
Test the different versions.



