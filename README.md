# CFI_Elec_Club_mini_task_3
Improvements in the projects
### Project 1. Ring with automatic sensor
In this project a ring is built so as to light up only when worn in the finger, otherwise it has to remain off. The basic design of the ring includes two 1.5 V batteries connected with a push button when worn in the finger gets pressed and the led light gets switched on otherwise push button keeps the circuit open. This basic design involved a problem that it could not be worn into finger for a long time as the push button causes pain in the finger as it is pressed when worn in the finger. So, we have to design a circuit that includes use of proximity sensor or any other sensor and microcontroller to turn the led on when the sensor sense the data after a certain threshold distance.
#### Ideation:
First Prototype:
<br />Circuit open==> Led Off==> Push button(On when finger presses it)==> Circuit closed==> Battery(3V)(current flows)==> Led On
<br />Suggest solution for the problem:
<br />Led off==> Batter(3V)(to power the circuit)==> Sensor(receives signal)==> Microcontroller==> Sets Led pin High
##### 1st approach
As used in the example, we'll be using an IR sensor which is smaell enough to fit in a small space like an led just to detect the finger. The IR sensor when it receives a signal will then be sent to ATTiny 45 microcontroller which is small enough and can work for less than 3V. We will be programming microcontroller to turn the led on after receiving signal from IR sensor. This approach has an advantage as the IR sensor can be purchased in a low cost.
##### 2nd aaproach
We'll use capacitive touch LED sensor developed by Visual Communications Company (VCC) that has size specification 15.0 mm x 15 mm.0 x 3.2 mm. That would be a very good method as the led will be on only when it is touched with conductor like human skin (if we wnat this quality in it too). As suggested in the example, we would be using ATTiny45 microcontroller which will be small and has a sleep mode and can work for less than 3V. These touch sensors have a special quality that these can operate anywhere between 2 to 5.5 V DC. We will be programming microcontroller to turn the led on after receiving signal from IR sensor.
<br />
&nbsp;

### Project 2. Control Systems for Reinforcement Learning - Hexapod
In Reinforcement Learning, one important part of the pipeline is to detect the state of the system at all Instances, This Hexapod has 18 DOF, your task is to Integrate different Sensors to the Hexapod and recreate the exact orientation of the Bot in a Computer , How would you plan to do so.
#### Ideation:
First Prototype:
<br />Motor(moves)==> IMU sensors(accelerometer or gyrometer)==> Microcontroller==> Data received by computer==> Combining data(received from sensors as well as initial data & orientation)==> Building exact orientation
<br />Suggested solution for the problem:
<br />Motor(moves)==> Motor encoders(detects how much motor has rotated in both direction)==> Microcontroller(arduino mega)==> Data received by computer==> Combining data(received from motor encoders as well as initial data & orientation)==> Building exact orientation
##### Approach:
So here instead of using IMU sensors and motors combined we'll be using motor encoders which will tell us how many degreeshave been rotated till now. Using motor encoders will have a slight disadvantage of cost which will be merely 50-100 Rs. more than that of IMU sensors + motors combined. But using motor encoders have more advantages over IMU sensors as these encoders can be controlled from computer as well as from remote controller as we'll be having the values of degree rotated easily. We just need to use 
<br /> The best advantage of using the motor encoders is that it would be so much easy to make it walk like a spider (using its first 6 legs), we can just feed the values of degrees to be rotated or the software can detect the values of angle the spider's legs to be rotated itself without any help and the hexapod can move according to the values given. And since, it can perform basic function of rotating with the help of remote control.
<br />The extra useful advantage of motor encoders over IMU+Motors is the coordination among the motors. As in the case of motors only, the motors might have different speeds for the same voltage and current so, instead of using the motors we'll use motor encoders which will ensure proper coordination of speed between the motors.
<br /> Now we'll be connecting microcontoller with computer with I/O pins or input and output to receive as well as to send data.
<br />These motor encoders are also a good option as they can tell us how much the motor (or leg) has rotated 'mechanically' may be by us, by surfaces or by jerk etc. This would also be detected by IMU sensors. But as you know the wires and hardware required would be less here.
<br /> We would be marking our hexapod with lines where the motors have 0 degree rotated in either direction and the orientation would be default as the initial condition.
<br />Using reinforced learning, we can make the orientation better and better with the time.
<br />The best smallest and cheapest motor which I could find online was [N20 12V 140RPM Micro Metal Gear Motor With Encoder](https://robu.in/product/n20-12v-140rpm-micro-metal-gear-motor-with-encoder/?gclid=CjwKCAjwte71BRBCEiwAU_V9h_m5qym33YjT6x3uZ8T9u38Bpe0aWku8FRcNEvrT1_TCTgnC0hfSCBoCfLoQAvD_BwE)
&nbsp;

This is not a part of problem but to make hexapod walk practically we can take the example of how the spider walks() in real life which could be helpful to make the hexapod walk fast: [https://www.youtube.com/watch?v=GtHzpX0FCFY](https://www.youtube.com/watch?v=GtHzpX0FCFY)
<br />
&nbsp;

### 3. MicroMouse Maze - TechSoc Challenge

































