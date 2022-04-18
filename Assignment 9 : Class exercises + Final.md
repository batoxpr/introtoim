# **ASSIGNMENT 9 - Class exercises + Final Project Idea** 🎨🔮✨ #
This week's assignment was to finish the exercises we did in class and come up with an idea for the Final project. 

For exercise one, it was pretty straightforward. We just had to remove the extra parts from the code we wrote in class and leave the analog sensor part.

**Task 1:**
[P5 Code](https://editor.p5js.org/insiyam/sketches/aZKDbrgGR)

*Arduino:*

const int POT = A0;
const int PR = A1;

void setup() {
  Serial.begin(9600);

}

void loop() {

 // send information to p5
  int potValue = analogRead(POT);
  int prValue = analogRead(PR);
  Serial.print(potValue);
  Serial.print(",");
  Serial.println(prValue);

}

For exercise two, I managed to modify the brightness value of the LED using analog value from the p5js, particularly the mouse. 
When the mouse is pressed, the light is dim. It's because the value was set to 240. However, It didn't work when I assigned multiple values to the LED using the KeyPressed function.

**Exercise 2:**

[P5 Code](https://editor.p5js.org/batoxpr/sketches/iUUjxHgDT)

*Arduino:*

const int LED = 3;
void setup() {
  Serial.begin(9600);
  pinMode(LED, OUTPUT);
  while (Serial.available() <= 0) {
    Serial.println("hello"); // send a starting message
    delay(300); //wait 1/3 second
  }
}

void loop() {

  // read information from p5
  if (Serial.available() > 0) {
    int ledValue = Serial.read();
    if (ledValue == 0) {
      analogWrite(LED, ledValue);
    } else {
      analogWrite(LED,ledValue);
    }  
  }
  }

I couldn't figure out why.

**Final Project Idea**

For the Final project, I want turn a plush Panda toy into a interactive toy that can be controlled from the P5js screen. I want the p5js visual to be also representative of the Panda itself. 
When I click on the nose from the p5 for example, the Panda's nose would light up. This is the initial idea. However, I;ll look at the past final projects from the previous students and will try to think of something more creative.
