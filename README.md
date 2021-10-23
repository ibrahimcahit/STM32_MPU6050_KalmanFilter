# Kalman Filter Implementation for MPU6050 on STM32 Nucleo Board

Kalman Filter Implementation for MPU6050 with STM32-Nucleo

I implemented a Kalman Filter via STM32CubeIDE using the NUCLEO-G431RB development kit and MPU6050 sensors.

Accelerometer and gyroscope sensors are used together to obtain Attitude information. The main reason for this is that when these two sensors work alone, their accuracy deviates so much that they cannot be used. Especially the case of "Gyro Drift" is one of the best examples of this.

Sensor Fusion aims to blend the different sensor data with the least error and is frequently used to obtain Attitude information. The Kalman Filter is also one of the popular methods used for Sensor Fusion.

Although this application is useful for one- or two-dimensional scenarios, it is insufficient in three-dimensional or "non linear" systems such as UAVs and unmanned systems.

In such scenarios, it may be necessary to use solutions like "Quaternion based Extended Kalman Filter". In addition, different sensor types or choosing a sensor module for each axis are other factors that increase accuracy.

Board used is: NUCLEO-G431RB

Detailed information: [NUCLEO-G431RB](https://www.st.com/en/evaluation-tools/nucleo-g431rb.html#overview)

## Circuit:

![](https://raw.githubusercontent.com/ibrahimcahit/STM32_MPU6050_KalmanFilter/main/img/20211023_232004.jpg)

## STMStudio GIF
![](https://raw.githubusercontent.com/ibrahimcahit/STM32_MPU6050_KalmanFilter/main/img/ZYpSiML59i.gif)
