# **ASSIGNMENT 7 - Analog Sensor with ARDUINO** 🎨🔮✨ #
This week's assignment was to build a circuit on Arduino, making use of the Digital and Analog components.

[Link to the Youtube video](https://youtu.be/JKJx49o2sLA)

**/Initial Idea**

In class, we have learned about the Analog input - specifically the Potentometer and Light sensor.
Based on that experience, I wanted to think of a creative way of using the Potentometer as a controller.
After some research, I figured out that I can use the Potentometer's input value and use that measure to assign functionalities.

**/Setting up the circuit**

To implement this possibility, I decided to use the value of Potentometer to control 4 array of LED lights. 
Maximum possible value of the Potentometer is 1024, which means it'd be 256, 512, 768, and 1024 respectively when divided by 4.
I wanted the LEDs to light up in this order, one after another as we tune the knob.

To achieve this, I first set 4 LEDs in array, connecting the short legs to 330 ohm resistors, and long legs to the positive wires. 
Each wire is in different color representive of the matching LED colors. All 4 wires are connected to different digital outputs on the board.

After this, I set the Potentometer on the other side of the breadboard. While I connected the left leg to the ground, right leg was connected to the positive. The middle leg is connected to the A5 analog input, distinctive by its white wire. 

**/Coding process**

Before starting the main code, I declared the integers of the LEDs, and the potentometer.
In the setup section, I declared the pinModes of each integers.

![image](https://github.com/batoxpr/introtoim/blob/a99fa049b9a06362589a6eeb48a2d4dbc7160428/assets/assignment%207_2.PNG)

In the loop section of the code, I first declared the potMeasure, which would read the value coming from the A5 analog input.

After that, I used the If and Else If conditionals to construct the code. Using the DigitalWrite function, I assigned High/Low states to the LEDs relative to the potMeasure value. As described previously, First LED is lit when the potMeasure value is below 256. Then second LED lights up as the value exceeds 256. third one as it reaches 512, and the fourth one on above 768. 

![image](https://github.com/batoxpr/introtoim/blob/dec963ddd85c4fec0989ee39452b2d8ac61a804b/assets/assignment%207.PNG)


**/Symbolism**

I used Potentometer as a metaphor for wallet, an item which we carry in our day to day lives. Each LED is representative of our happiness level. When all four LEDs are on, it's a state of maximum level of happiness. Overall, this piece is a social commentary on how our happiness is dependent on the amount of cash we have in our wallet.



