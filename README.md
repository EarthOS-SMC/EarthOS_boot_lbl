# EarthOS little bootloader
This is a part of EarthOS; the build system uses this repository for the `/boot.smc` file.

This bootloader starts the kernel located in `/boot`. It doesn't have any multi-boot support, and will never have.
Use EBL for multi-boot things, this is just for a fast installer booting.

## Building from source

Clone this repository using this command:

`git clone https://github.com/EarthOS-SMC/little-bootloader`

Then, go to the source code directory:

`cd little-bootloader`

Before the build process, you need to clone the PowerSlash compiler too:

`chmod +x sync.sh && ./sync.sh`

To build the bootloader,

`./build.sh`


The binary will be saved in the `image` file.

## Reduce output

You can reduce the output by putting `1` in the `reduce` file:
`echo 1 > reduce`
