# Virtual Hand Simulator

## Overview
A Virtual Hand Simulator developed using Unity Engine. It uses data collected from flex sensors and an MPU6050 accelerometer through an Arduino. The data is mapped to a Blender model of a hand to simulate the curl of the thumb, index, and middle fingers, as well as the hand's orientation in 3D space using quaternion values from the MPU6050.

## Features
- Tracks and maps thumb, index, and middle finger curls.
- Maps hand orientation in 3D space.
- Real-time simulation in Unity.

## Hardware Requirements
- Arduino (e.g., Arduino Uno)
- Flex sensors
- MPU6050 accelerometer
- Jumper wires
- Breadboard

## Software Requirements
- Unity
- Blender
- Arduino IDE
- MPU6050 Library for Arduino

## Setup
1. **Arduino Configuration**:
   - Connect flex sensors to Arduino's analog pins.
   - Connect MPU6050 to Arduino via I2C.
   - Install the MPU6050 library in Arduino IDE.
   - Upload the Arduino sketch to read sensor data and send it via serial communication.

2. **Blender Model**:
   - Create or download a hand model in Blender.
   - Ensure the model has bones and rigging for the thumb, index, and middle fingers.

3. **Unity Integration**:
   - Import the Blender hand model into Unity.
   - Create a Unity script to read serial data from the Arduino.
   - Map the flex sensor data to the finger bones in Unity.
   - Use quaternion data from the MPU6050 to orient the hand model in 3D space.

## Usage
1. **Connect the Hardware**:
   - Connect the Arduino to the computer and power it on.
   - Open the Unity project and run the scene with the hand model.

2. **Run the Simulator**:
   - Start the Unity scene to initialize the virtual hand.
   - Move your physical hand with sensors attached.
   - The virtual hand model will replicate the movements in real-time.

