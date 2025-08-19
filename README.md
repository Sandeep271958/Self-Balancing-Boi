# Self-Balancing Robot

<!-- This is a comment -->


<!-- ![Self-Balancing Robot Prototype](./assets/robot_prototype.jpg)  
*A picture of the self-balancing robot prototype.* -->


---

## Overview
This repository documents my **progress in building a self-balancing robot** that can be controlled wirelessly using the **EZ-GUI mobile application** via Bluetooth.  

The robot primarily uses **stepper motors** for motion and balance, with feedback from a **6-axis gyroscopic sensor**. A **PID controller** stabilizes the system in real-time.  

---

## Key Features
- **Mobile Control** – Controlled via the **EZ-GUI Android app** using Bluetooth.  
- **Self-Balancing** – Uses a **6-axis MPU6050 gyroscopic sensor** for orientation and acceleration feedback.  
- **PID Control** – Implements a PID loop for real-time balance stabilization.  
- **Stepper Motor Drive** – High torque and precision control with **A4988 stepper drivers**.  
- **Custom PCB** – Neatly integrates all components (Arduino Nano, BT module, motor drivers, connectors).  
- **Reliable Power** – Powered by an **11.1V 2200mAh 3S 40C Li-Po battery**.  

---

## Hardware & Components
- **Microcontroller**: Arduino Nano  
- **Bluetooth Module**: HC-05  
- **Motor Drivers**: A4988 stepper drivers  
- **Motors**: Stepper motors  
- **IMU Sensor**: MPU6050 (6-axis gyro + accelerometer)  
- **Battery**: 11.1V 2200mAh 3S 40C Li-Po  

---

## Custom PCB
I designed a **custom PCB** to connect and hold all the essential modules and components:  
- Arduino Nano  
- HC-05 Bluetooth module  
- A4988 Stepper motor drivers  
- MPU6050 gyroscopic sensor  
- Connectors for power and motors  

<!-- ![Custom PCB](./assets/custom_pcb.jpg) -->

---

## Control System
- Robot orientation data is continuously collected from the **MPU6050 sensor**.  
- A **PID algorithm** calculates corrections required to keep the robot upright.  
- The correction signals are sent to **stepper motors via A4988 drivers**.  
- Commands from the **EZ-GUI app** are received through the **HC-05 Bluetooth module** and processed by the Arduino Nano.  

---

