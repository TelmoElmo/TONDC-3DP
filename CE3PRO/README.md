# TONDC-CE3PRO
 Tonbridge School Digital Creativity Department Creality Ender 3 Pro

The machiene is heavily modified. Current changes include:

- Installation of Klipper Firmware (Communicating via. UART)
- Installation of BTT SKR Mini E3 V3.0 Mainboard
- Installation of Teaching Tech Ender 3 Rear Mount Electronics case (w. integrated Pi 3)
- Configuration of a USB webcam via. crowsnest for continuous video monitoring
- Installation of MicroSwiss NG REVO Direct Drive toolhead
- Installation of BTT Eddy Duo ABL Probe (used for Z Homing)
- Installation of BTT EBB 42 CAN board (running over USB)
- Installation of KevinAkaSam Ender 3 Belted Dual Z Mod (w. linear rails) *IN PROGRESS* (https://kevinakasam.com/dnmd20-2/)

Input shaping and pressure advance have not been calibrated. There is an accelaromotor in the EBB 42 board, however on an i3 configuration this only allows for tuning in X, not Y.

To allow klipper to communicate via the raspberry Pi's UART Pins, several device tree level changes need to be made. The easisest way to make these changes ids to flash from an image which has already completed all these changes. MainsailOS would therefore be recomended. If an alternate interface, such as OctoPrint or Fluidd is prefered, flash an image of Mainsail OS, install KIAUH (dw-0/kiauh), uninstall the mainsail interface and install anything else desired.


Damage List:
BTT SKR Mini E3 V3 board - Micro USB port detatched, SD port damaged but usable if held in place. Marlin not advised for these reasons. Previous repair attempted to resolder USB port unsuccesful. Could always swap with identical unit in the Enderr 5 S1.
Strong stiffness in REVO nozzle, believed to be isolated to specific nozzle and not toolhead.