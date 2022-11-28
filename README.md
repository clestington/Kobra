# Changes on Marlin Firmware to use after klipper UART mod

## Goal:
Using Marlin FW after the hardware mod on TMC2209 UART adress according to:
https://www.reddit.com/r/anycubic/comments/ynvbj0/anycubic_kobra_working_config/?sort=new


1) Change of UART Adress
    To use UART in Klipper the adress of TMC2009 driver from X stepper needs to be changed
    a) resistor for X driver has to be resoldered to change adress from 0 to 3
    b) slave_adress in Marlin FW (Configuration_adv.h) has to be changed if

2) Change startup sound to be more quiet // In progress


## Notes:

-> Compiling firmware based on anycubics anycubic.uvprojx file (Anycubis uses Keil uVision5)
    https://www.reddit.com/r/anycubic/comments/y2waxu/tutorial_how_to_build_anycubic_marlin_source_code/