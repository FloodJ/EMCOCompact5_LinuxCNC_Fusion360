# EMCO Compact 5 PC Lathe - LinuxCNC - Fusion360
Configuration for Fusion 360 and LinuxCNC to control an EMCO Compact 5 PC lathe.

## Background
The EMCO Compact 5 PC was originally programmed and controlled using proprietary software that was licensed with a parallel port dongle. The goal of this project is to greatly improve the functionality by assembling the necessary instructions, configuration files and workflow processes to control the lathe using Fusion 360 and LinuxCNC.

## Requirements
* A PC (can be tested for suitability using the LinuxCNC live boot image)
* A parallel port (PCIe, not a USB adapter)
* A 4GB USB stick (for the LinuxCNC image)
* A stock EMCO 5 PC Lathe

## Process Overview
1. Run the latency test from the LinuxCNC live image to confirm that the PC is suitable.
2. Install LinuxCNC.
3. Copy the config files from this repository into the linuxcnc user's home directory.
4. Edit the .hal file to use the correct parallel port address.
5. Measure your tooling and pre-fill the tool offsets table.
6. Touch off to confirm tool offsets.
7. Configure tooling in AutoDesk Fusion.
8. Generate NC files in Autodesk Fusion.
9. Load and test NC files in LinuxCNC.

## Resources
* My [video tutorials](https://youtube.com/playlist?list=PLcKM6L7ggUSsdoUyl2B9aQ3vQ-EnV4jcR&si=2oiRL0iOqzVm240o)
* [Getting LinuxCNC](http://linuxcnc.org/docs/stable/html/getting-started/getting-linuxcnc.html)
* The [LinuxCNC Latency Testing](https://linuxcnc.org/docs/stable/html/install/latency-test.html) page
* The [parallel port card}(https://www.startech.com/en-au/cards-adapters/pex1p2) that I used
* Samco's original [LinuxCNC config files](https://www.cnczone.com/forums/emco-lathe/186598-machinist-software.html#post1818116)
* [ISO decoder for toolholders](https://www.carbideanddiamondtooling.com/Indexable.Turning.Toolholder.Nomenclature)
* [ISO decoder for inserts](https://www.carbidedepot.com/formulas-insert-d.htm)
* Blondihacks' [Metal Lathe Tutorial 21 : Speeds & Feeds](https://youtu.be/NrcDr2WO6Ho?si=jX-Vb-jrdoQot7dv)

## To Do
* Complete video on creating NC files in Fusion.
* Complete documentation.
* Update half-step configuration file to work with LinuxCNC 2.9.x

