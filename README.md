Setup & Installation
1) STM32 Setup: 
Flash the provided firmware to your STM32 board

2) Connect HC-05 module to USART3 pins:
   TX → RX (PB11)
   RX → TX (PB10)
   VCC → 3.3V 
   GND → GND

3) MATLAB Setup: 
Ensure MATLAB has Instrument Control Toolbox
Pair HC-05 with your computer (default PIN: 1234)
Run the MATLAB GUI script
Select the correct COM port for Bluetooth connection

4) Usage:
Power on the STM32 system
The HC-05 module will enter pairing mode
Launch MATLAB GUI and establish Bluetooth connection
View real-time status messages:

Initial welcome message: "STM32 HC-05 Connected. Welcome to MATLAB GUI Test!"
Periodic updates: "Still running..." every 2 seconds


Note: In macOS it requires the installation of blueutil for turning on the bluetooth. Which also creates another problem, the HC05 module connects for first two runs then it won't. I tried Forgot device, then connecting again. However the problem arises again after two runs. The problem is related to MATLAB interaction with macOS. 
