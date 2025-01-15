# TONDC-CE5S1
 Tonbridge School Digital Creativity Department Creality Ender 5 S1

The machiene is heavily modified. Current changes include:

- Installation of Klipper Firmware (Communicating via. UART)
- Installation of BTT SKR Mini E3 V3.0 Mainboard
- Removal of stock touch screen LCD display
- Installation of LCD enclosure *IN PROGRESS*
- Configuration of a USB webcam via. crowsnest for continuous video monitoring
- Installation of BTT Eddy ABL Probe (used for Z Homing)
- Installation of MicroSwiss NG Direct Drive toolhead
- Configuration of sensorless homing on X

Input shaping and pressure advance have not been calibrated.

To allow klipper to communicate via the raspberry Pi's UART Pins, several device tree level changes need to be made. The easisest way to make these changes ids to flash from an image which has already completed all these changes. MainsailOS would therefore be recomended. If an alternate interface, such as OctoPrint or Fluidd is prefered, flash an image of Mainsail OS, install KIAUH (dw-0/kiauh), uninstall the mainsail interface and install anything else desired.

To achieve the instalation of a toolhead with a nozzle signifgantly higher than the stock toolhead, it was nesecarry to raise the bed closer to the nozzle. This process involved the removal of the timing belts on the left had side of the Y axis and the asociated linking rod attached to the Left hand side of the Y stepper motor, and the elevation of the Z stepper motor through the use of M5 screws, T-Nuts, and the Motor Riser.stl part in the hardware section. This should be printed with a high infil in a stiff material not suceptable to warping (i.e. PETG, ABS, no PLA, no TPU)

To mount the Eddy Probe, Print and install the Eddy MountNG.STL file. Models found online were only compatible with the NG REVO toolhead, which has a lower nozzle height and therefore means lower mounting holes provide sufficient clearence between the probe and the build plate. The STL raises the probe higher, providing adequate clearence. If you are in any way able to design a better part, submit a pull request removing the existing STL and adding your new design. Leave the STL name as is.

The stock mainboard is not used, and it's mounting holes are not compatible with the BTT SKR Mini E3 V3.0 Mainboard. Therefore, the SKR Bracket S1.STL file, and M3 Screws, are required. The I/O ports are not accessible. You may wish to cover these with black electrical tape.