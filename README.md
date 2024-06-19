This Repo has my progress for the self balancing robot, That can be comtroled using a mobile application called "EZ-GUI" via bluetooth.
it mainly uses STEPPER motor for its motion and to balance.
It uses Arduino Nano as the main Controller, It Communicates with the mobile app and recieves commands with the help of HC-05 BT module.
Im using a 6-axis gyroscopic sensor to get the orientation and Acceleration of the robot, this data will be used to stabilise the robot Using PID.
Ive designed a Costum PCB for the robot to connect and hold all the essential modules and components like Arduino nano, HC-05 BT module, A4988 Stepper motor Driver, MPU6050 6-axis gyro sensor, connectors.
Im using a 11.1V 2200mah 3S 40C Li-po battery as the power source for the robot.
