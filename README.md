# EMCO Compact 5 PC Lathe - LinuxCNC - Fusion360
Configuration for Fusion 360 and LinuxCNC to control an EMCO Compact 5 PC lathe.

## Background
The EMCO Compact 5 PC was originally programmed and controlled using proprietary software that was licensed with a parallel port dongle. The goal of this project is to greatly improve the functionality by assembling the necessary instructions, configuration files and workflow processes to control the lathe using Fusion 360 and LinuxCNC.

## Requirements
- A PC (can be tested for suitability using the LinuxCNC live boot image)
- A parallel port (PCIe, not a USB adapter)
- A 4GB USB stick (for the LinuxCNC image)
- A stock EMCO 5 PC Lathe

## Process Overview
1. Run the latency test from the LinuxCNC live image to confirm that the PC is suitable.
2. Install LinuxCNC.
3. Copy the config files from this repository into the linuxcnc user's home directory
4. Edit the .hal file to use the correct parallel port address
5. Measure your tooling and fill in the tool offsets table
6. Generate NC files in Autodesk Fusion

## Resources

## To Do
- Complete video on tool offsets and machine set-up.
- Complete video on creating NC files in Fusion.
- Complete documentation.
- Update half-step configuration file to work with LinuxCNC 2.9.x

