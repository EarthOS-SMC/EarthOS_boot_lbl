# EarthOS little bootloader
This is a part of EarthOS; the build system uses this repository for the `/boot.smc` file (boot partition).

This bootloader starts the kernel located on the first (boot) partition. It doesn't have any multi-boot support, and will never have.
Use EBL for multi-boot things, this is just for a fast installer booting.
