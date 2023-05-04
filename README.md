# **Forest Fire Detection with SMS Alerts**

The primary motivation for designing a fire detection system was the devastating news of the Australian Forest Fires in 2019-2020. 
A forest fire detection system is an embedded system project that involves detecting fire in the forest and then alarming or informing us about the danger by sending an SMS. Detection of fire in a forest initiates at any of the nodes planted on a tree inside the forest. The forest has a network of nodes placed at suitable distances from each other. The nodes have the capability to communicate through devices (RF module in our case) and by using Arduino. If any change is found, above a threshold value, in the atmospheric parameters (temperature rise, contamination of air with smoke, etc.) near a node (source node), the information is passed to the nearest intermediate node until it reaches the main/head terminal. The main/head terminal uses a GSM modem to pass the information to a cell phone (the forest fire monitoring center).

## Table of Contents
    1. Description
    2. Hardware Requirement
    3. Software Requirement
    4. Block Diagram
    5. Circuit Diagram
    6. Working of the System
    7. Result
    8. Future Scope
    
## Description
In the present era, wildlife and forest departments are facing the problem of movement of animals from forest area to residential area. The number of trees has reduced drastically from the forest that creates an unhealthy environment for animals to survive in the forest. It has been found in a survey that 80% losses are caused due to fire. This could have been avoided if the fire was detected in the early stages. This project proposes a system for tracking and alarming for the protection of trees against forest fires

## Hardware Requirement
### 1. Arduino Uno

 ![arduino](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR2YjUpS0aymH4CJbBzL7sK1iVgSb4c9RXffw&usqp=CAU)
 
### 2. DHT11 Sensor (Temperature & Humidity Sensor)

![dht11](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQRfe5IC9jjOpvWSKQMyLQT4_BWKfgmc_6-dQ&usqp=CAU)
### 3. GSM Module
![gsm](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQQ5s9jmo_pSycY42_YG51sb4C_aIe7MmhmlsmsxZvXXOhpyQdGWm7siKM4YOdPg-JreZ8&usqp=CAU)
### 4. GPS Module
![gps](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTzFJfUnbUjnncKluLASc7AFWv8w-1dJWvaLw&usqp=CAU)
### 5. RF Module
![rf](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTonRxyscyzwWcb_s5KpxfHpK6CU0KWMLpLHg&usqp=CAU)
## Software Requirement
### 1. Arudino IDE
It is a free IDE that can be downloaded from https://www.arduino.cc/en/software
## Block Diagram
![bd](https://www.linkpicture.com/q/bd_3.png)
## Circuit Diagram
![ckt](https://www.linkpicture.com/q/ckt-diagram.png)
## Working of the System
The forest fire detection module works in three different stages. The first stage consists of reading external environmental parameters like temperature and smoke. The first step is designed with the help of some sensors that sense and converts analog data to digital data. The sensors read parameters like temperature, humidity and air quality and then send this information to the next nearest node. This process continues until the information reaches the final node or the main terminal, the second stage of the overall process. The third stage consists of the transmission of the information to the forest fire monitoring unit. Each node has a temperature and humidity sensor, a smoke sensor and a microcontroller unit. Arduino is a microcontroller device. The sensors interact with the Arduino and store the information for the comparison process. There is a predefined threshold value for each of these parameters. The microprocessor compares the sensor values at regular intervals of time with the threshold values. Based on the comparison if the input values of sensors exceed the threshold the node transmits the information to the next nearby node which again in turn transmits the information to the other nearby node. In this way, the message flow is regulated in this model.

# Result
![res1](https://www.linkpicture.com/q/result1_major.png)

# Future Scope
The Project can be extended for addition of
1. A module by which water can be supplied so as to control the fire till the emergency team arrives
2. Development of technology in order to reduce the number of microcontrollers used.
3. Developing a faster means of communication in order to cover the large area of detection system in forest







