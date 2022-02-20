# **ASSIGNMENT 4 - GENERATIVE TEXT on P5.JS** 🖼️ #
Here's the [link](https://editor.p5js.org/batoxpr/full/BhxH4QVfa) to my Assignment 4: Generative text! 
Along with the [Code Link](https://editor.p5js.org/batoxpr/sketches/BhxH4QVfa)

First, I made an object named "Eye" that contains constructor, drawEye, and moveEye functions. The constructor contains the x and y position of the eye. 
The draw eye function uses those constructor values to draw multiple shapes, which come together to draw the eye. 
Each shape has their separate fills. I used noise function for the color changing iris.

The move eye function changes the x and y coordinates of the eye using noise function. I used a pre-declared value k for both noise usages (fill and movement).
By using the the "for loop" function, I made an array of 9 different eyes in random coordinates. Then I used mouseIsPressed to move the eye when it's pressed. When the mouse is not pressed, it just draws 10 eyes in random places. I wanted all 9 eyes to move, but because I used noise function, they were overlapping. I couldn't really find solution to this. 

Regardless, it was a good practice for making use of various topics we've learn in class.
