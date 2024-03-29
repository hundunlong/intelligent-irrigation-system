# Intelligent Irrigation System
Details in this [Report](Technical_Report.pdf) 
## Members
- Weiwei(2740470W) https://github.com/wayne-weiwei
- Jinhai Hu(2822462H) https://github.com/JJinhai
- Li Meiwen(2429437L) https://github.com/IrinLi
- Qian Xiaoyu(2824018Q) https://github.com/hundunlong (most are committed as Qian,Xiaoyu )

# Irrigation System
![Irrigation System](pics/system.jpg)
The Irrigation System is designed to automatically water plants based on their needs. It uses sensors to monitor soil moisture levels and adjusts the watering schedule accordingly.
## Social Medium
[![youtube](pics/youtube.png)](https://www.youtube.com/@Team39Intelligent)


## Hardware Components

- Soil moisture sensor: Measures the moisture content in the soil.
- Water pump: Delivers water to the plants when needed.
- Microcontroller: Collects data from sensors and controls the water pump.

![Irrigation System Diagram](pics/Soil_sensor.png)

# Intelligent Car System

The Intelligent Car System is responsible for the mobility of the overall system. It allows the irrigation system to move around and cover a larger area.

## Hardware Components

- Motors: Provide motion to the car.
- Wheels: Enable the car to move.
- Battery: Supplies power to the motors and other electronic components.


# Overall System Assembly
![OverallSystemAssembly](pics/Overall_system.png)
![OverallSystemAssembly2](pics/struction.png)
The Overall System Assembly combines the Irrigation System and the Intelligent Car System to create a mobile, automated solution for watering plants.

## System

- Irrigation System: Takes care of watering the plants.
- Intelligent Car System: Provides mobility to the irrigation system.

![Overall System Assembly Diagram](pics/motor.png)
![Overall System Assembly Diagram2](pics/servo.png)
![Overall System Assembly Diagram3](pics/PCA9685.png)

# Soft Design and Function

The software part of the system ensures seamless integration between the irrigation system and the intelligent car system.

## 1) Path Planning
![pathplaning](pics/pathplaning.png)
The system uses path planning algorithms to navigate efficiently and avoid obstacles while moving from one plant to another.

## 2) Infrared Sensor Activation
![Infrared Sensor](pics/Infrared_sensor.png)
Infrared sensors detect obstacles and help the system navigate safely.

## 3) Light-sensitive Sensor
![lightsensor](pics/lightsensor.png)
The light-sensitive sensor measures the ambient light, ensuring optimal lighting conditions for plant growth.

## 4) Irrigation System
![Flowchat](pics/Flowchat.png)
The software component of the irrigation system receives data from the soil moisture sensors and controls the water pump accordingly.

# The process of flower growing
![seed](pics/seed.jpg)
![seedling](pics/seedling.jpg)
![flower](pics/flower.jpg)

# compile commands
```bash
// module test
g++ -o testMotor testMotor.cpp pca9685/pca9685.c -lwiringPi -pthread 
./testMotor 2000 1/0
```
```bash
// main
g++ -o main main.cpp pca9685/pca9685.c -lwiringPi -pthread
```
```bash
// front
cd client
npm install // install the dependencies
npm start // test in localhost
npm run build // mkdir dist and build
```
```bash
// server
cd server
g++ -o http http_server.cpp -pthread
```

# key word
Raspberry C++ PCA9685
