# 2021 BEST
Code for BEST Robotics

**Sourced From Robotics Club Engineering Notebook:** 
## Software Design
Every code segment started by defining the mechanical requirements for the robot. Afterwards, pseudocode was developed to plan the objective of each part of the program and what the result would be for the robot. The design and build team was consulted to confirm any necessities before the programming team began coding segments in Robot-C. The objectives were two drive motors, one arm motor, two actuator servos and autonomous driving. Simple motor and servo code was developed as each part of the robot was built, along with simulated limits. After modifying the code, it was tested for objectives such as speed and driver ease. A controller manual was given to the driver team to review and work out with the programming team to maximize comfort of use before being finalized. This manual would be studied and referred back to by the driver team to practice for maximum performance before game day. One method for the autonomous driving objective using the IR sensors was also designed, a distance-evaluating algorithm and an action initializing encoder. For distance-evaluating, one algorithm was written using different numbers of sensors: a two-sensor array, after referring to the design and build team.  For the encoder solution, a distance tracking method utilizing the limit switch was developed, and a PID loop was used for accuracy. After each code segment was tested and modified, the methods were implemented into the robot code. As the software was written, thorough but concise comments were added throughout the program. Every block was specifically named for its function. This allows for a better understanding of the function of the program and enables anyone, software designer or not, to edit the software with ease.

## Test and Debug
As code was written and implemented to the Cortex, a simple process was followed to evaluate it. First, all the motors were tested to confirm they were correctly oriented. If not, motors were simply reversed in the program. Second, all digital inputs were tested for functionality. It was planned that while running the autonomous program, the behavior of the IR sensors was evaluated. If errors were found, the wiring was checked and if the devices functioned, the code logic was updated for errors. If autonomous was working correctly, the behavior of the limit switch was tested by pressing it. The same process was then repeated to test and debug the limit switch. The software was repeatedly tested and evaluated until the desired results were achieved.

## Version Tracking and Code Release
Documentation of code release is a vital part of understanding and communicating software updates. It is important to be aware of what changes have been made, who made them, and when they were implemented. The robot documentation, which we posted and updated on [GitHub](https://github.com/jpx32/BEST-2021/), allowed team members to keep track of current and completed requirements. Whenever build objectives were met or changed, documentation allowed the team to keep a schedule of the design and revert to old versions if needed. Software releases were tracked with version numbers to ensure the program running on the robot was up-to-date.

## Simulation
As designs were being created,  the programming team used software which contained built-in functions that could simulate the output of the Robot-C code. With the introduction of the autonomous game objective, the ability to simulate sensor values through the distance evaluating algorithm was crucial. With simulation of the two IR sensors, the programming team was able to run several test cases without having to upload code to the robot. The simulation also allowed for the team to tune initial PID values for the encoder.

**Original Source:**
|Button/Switch|Action|
|--|--|
|L1|Top Pulley Motor Down|
|L2|Top Pulley Motor Up|
|R1|Claw Open|
|R2|Claw Close|
|7L|Half Speed|
|8R|Quarter Speed|
|7D|Reset Speed Divisor|
|8D|Reset Speed Divisor|
|Joystick 3|Motion (Left Wheel)|
|Joystick  2|Motion (Right Wheel)|
|7U|Light Pole Magazine Actuator Close|
|8U|Light Pole Magazine Actuator Open|
|7R|Autonomous (IR)|
|8L|Reset Variables Used for Autonomous Portion|
