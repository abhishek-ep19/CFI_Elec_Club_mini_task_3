# CFI_Elec_Club_mini_task_3
Improvements in the projects
### Project 1. Ring with automatic sensor
In this project a ring is built so as to light up only when worn in the finger, otherwise it has to remain off. The basic design of the ring includes two 1.5 V batteries connected with a push button when worn in the finger gets pressed and the led light gets switched on otherwise push button keeps the circuit open. This basic design involved a problem that it could not be worn into finger for a long time as the push button causes pain in the finger as it is pressed when worn in the finger. So, we have to design a circuit that includes use of proximity sensor or any other sensor and microcontroller to turn the led on when the sensor sense the data after a certain threshold distance.
##### 1st approach

##### 2nd aaproach
We'll use capacitive touch LED sensor developed by Visual Communications Company (VCC) that has size specification 15.0 mm x 15 mm.0 x 3.2 mm. That would be a very good method as the led will be on only when it is touched with conductor like human skin (if we wnat this quality in it too). As suggested in the example, we would be using ATTiny45 microcontroller which will be small and has a sleep mode and can work for less than 3V. 
