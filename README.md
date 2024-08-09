# Accident-Notification-System
Overview
This project implements a vehicle crash detection system using an Arduino board, GPS module, GSM module, and MPU6050 accelerometer. The system detects sudden changes in acceleration, indicating a potential crash, and sends an SMS alert containing the vehicle's location to a predefined phone number.

**Components:**
Arduino Uno board
MPU6050 accelerometer
GPS module (e.g., NEO-6M)
GSM module (e.g., SIM900)
Breadboard and jumper wires

**Setup Instructions:**
Connect the MPU6050 accelerometer, GPS module, and GSM module to the Arduino board following the wiring diagram provided.
Upload the Arduino sketch (vehicle_crash_detection.ino) to the Arduino board.
Ensure that the GSM module has an active SIM card with SMS capabilities and that the GPS module has a clear view of the sky to acquire GPS coordinates.
Power on the system and wait for the initialization process to complete.
In case of a crash event, the system will detect the sudden acceleration change, retrieve the GPS coordinates, and send an SMS alert to the specified phone number.
Usage
After setup, the system continuously monitors the vehicle's acceleration.
If a crash event is detected (acceleration exceeds a threshold), an SMS alert is sent to the configured phone number.
The SMS alert contains the vehicle's current GPS coordinates and a Google Maps URL for location visualization.

**Dependencies**
TinyGPS++ library: https://github.com/mikalhart/TinyGPSPlus
SoftwareSerial library: https://www.arduino.cc/en/Reference/softwareSerial
MPU6050 library: https://github.com/jrowberg/i2cdevlib/tree/master/Arduino/MPU6050
