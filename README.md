# Smart_car
This project was made in order to open the windows of my car from a mobile app.
#01_canSniffer_Arduino
This creates an interface between the arduino and the GUI. If the RANDOM_CAN define is set to 1, this code is generating random CAN packets in order to test the higher level code. The received packets will be echoed back. If the  RANDOM_CAN define is set to 0, the CAN_SPEED define  has to match the speed of the desired CAN channel in order to receive and transfer from and to the CAN bus.
#02_canSniffer_GUI
This was made in order to see the CAN messages and to be able to decode it. Using some reverse-engineering we could create a dictionary of received CAN messages to see what to transmit to get the desired outcome.

HW used:
-> Arduino UNO R3
->MCP2515 CAN driver
->OBS-2 plug
->OBD-2 Y Splitter

TBD:
-integrate an arduino bluetooth module to our arduino setup made in the car.
-create a mobile app fo android to send action via phone to the car.
