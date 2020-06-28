# Servos - Position control motors!
## Table of contents
* Introduction
* Working
* Feedback mechanism
* Oscillations
* Servo Jitters!

### Introduction
Servos are position control motors which are very precise, better servomotors are used in car steering, control surfaces of a plane, rudder of boats etc ... inexpensive servos are used in small scale robotics.
### Working
Servos consist of mainly 4 parts: 
  1. DC motor - Less torque, high speed
  2. Gearbox - These convert to high torque and low speed
  3. Potentiometer/rotary encoder - They are directly connected to output, hence have an acuurate sense of postion which the servo moved to.
  4. Microcontroller - It recieves input and moves the dc motor to appropriate position using feedback from potentiometer/rotary encoder.
### Feedback Mechanism
The poteniometer sends signal to the microcontroller on which position it has moved to, and if the position it moved to does not match with the input(may happen due to external factors) the microcontroller moves the servo to where it should be moved. This process repeats continuously to very small errors.
### Oscillations(optional for physics enthus - PH1010 for insti peeps)
Whenever the servo overshoots, using a H-bridge which is integrated to microcontroller, it reverses the current hence the dc motor... thus giving a backward torque. Which in PH1010 terms is "FORCED DAMPED OSCILLATIONS"
### Servo Jitters!
Usually the overshoots are very small, and the oscillations happen withing very less time to nearly 0 error, hence our naked eye cannot spot the oscillations.
But when the load is too high, the torque will not suffice to oppose the inertia of the moving arm, hence the overshoots become large...giving us servo jitters! which our eye can spot easily
#### Solution to jiiters?
Use powerful servos XD
