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

To achieve the instalation of a toolhead with a nozzle signifgantly higher than the stock toolhead, it was nesecarry to raise the bed closer to the nozzle. This process involved the removal of the timing belts on the left had side of the Y axis and the asociated linking rod attached to the Left hand side of the Y stepper motor, and the elevation of the Z stepper motor through the use of M5 screws, T-Nuts, and the Motor Riser.stl part in the hardware section. This should be printed with a high infil in a stiff material not suceptable to warping (i.e. PETG, ABS, no PLA, no TPU)

To mount the Eddy Probe, Print and install the Eddy MountNG.STL file.

The stock mainboard is not used, and it's mounting holes are not compatible with the BTT SKR Mini E3 V3.0 Mainboard. Therefore, the SKR Bracket S1.STL file, and M3 Screws, are required. The I/O ports are not accessible. You may wish to cover these with black electrical tape.