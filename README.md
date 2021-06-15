## Motor Controller

**General Info:**

Cascadia Rinehart PM100 DX

Input: 100-360Vdc 250A (Const), 350A (Peak)

Output: 300A (RMS Cont), 350A (RMS Peak)

HW Version: 23450

HW ID: G3

Motor Type: 82

### About datasheet:

Please follow the datasheet in [/doc](/doc) folder, not the newer one from Cascadia


### How to calibrate resolver settings for motor 

Before calibration, the EPPROM value should be saved as a backup

For detail of calibration process, please follow this [guide](/doc/RMS Resolver Calibration Process.pdf)


After calibration, the entire EPPROM value should be export to [/log](/log) 

### How to use RMS GUI

RMS GUI is a standalone GUI software for check motor controller info and errors and tune settings <br><br/>
RMS GUI is assotiate with firmware version and system pre-defined values, and those two have to match in order to get correct reading


### How to flash the firmware

Pre-requirement: 

Install [C2 Programmer](/tools)

Step1: Turn off motor controller 

Step2: Connect RS232 adapter to motor controller

Step3: Put program swith on motor controller harness and switch on

Step4: Open C2 Programmer, select com port and hex file

Step5: Target 28234, Options 30MHz

Step6: Swith motor controller program switch off and power cycle motor controller 

Step7: Open RMS GUI and verify the EPPROM value
