# TONDC-CE5+
 Tonbridge School Digital Creativity Department Creality Ender 5 Plus

The machiene is heavily modified. Current changes include:

- Installation of Klipper Firmware (Communicating via. UART)
- Installation of BTT Octopus V1.1 Mainboard
- Installation of second extruder motor for potential dual extrusion prints
- Configuration of a USB webcam via. crowsnest for continuous video monitoring
- Installation of Dual Duct Filament mixing toolhead (currently removed)
- Installation of Mercury 1.1 Custom Electronics enclosure (in progress)
- Toolhead connections (exc. motor) localised at the end of the toolhead umbilicle. Secure w. Zip ties. You will need to crimp down cables to much shorter lengths using the crimping set.

There are currently exposed electronics on the machiene. Whilst we have made our best efforts to isolate all conductive areas, we cannot garuntee your safety. Please therefore exercise extreme caution when working arround this machiene. When complete the 1.1 Electronics enclosure should provide some extra safety and better cable management.

Input shaping and pressure advance have not been calibrated.

To allow klipper to communicate via the raspberry Pi's UART Pins, several device tree level changes need to be made. The easisest way to make these changes ids to flash from an image which has already completed all these changes. MainsailOS would therefore be recomended. If an alternate interface, such as OctoPrint or Fluidd is prefered, flash an image of Mainsail OS, install KIAUH (dw-0/kiauh), uninstall the mainsail interface and install anything else desired.

We have had bad luck so far with the mixing toolhead, and are exploring a potential custom AMS option. Not yet sure. No filament cutter is available.

Damage List:
-BTT Octopus - One fan MOSFET blown, fan 0. Port is dead. Fortunately there is no shortage of fan ports on the octopus. Refer to board schematics