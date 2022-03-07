# **MID-TERM GAME PROJECT DOCUMENTATION** 🎨🔮✨ #

Current version: https://editor.p5js.org/batoxpr/sketches/Sliroo3bj
I'm still updating the documentation

After getting a feedback on the dressup game idea, I decided to go for a completely different concept. The new game will be a "shoot 'em up" arcade game inspired by the classic Space Invaders. The name of the game will be "Emoji war" and It'll be a battle between Heart-eye emoji and Evil face emojis. The characters will be animated. Because I realized that there should be some sort of gameplay or challenge to it, I decided to go for this concept.

//**ASSETS**

For the font, I've found the following from GoogleFonts library. I wanted to go for a pixelated retro gaming theme. Therefore it fits well.
Insert image here
For the characters, I'm using the following two I've found from google
Insert images here
For the sounds, I;ve found the following:
(win)https://freesound.org/people/Leszek_Szary/sounds/171671/
(lose)https://freesound.org/people/myfox14/sounds/382310/
(shoot)https://freesound.org/people/AlaskaRobotics/sounds/221091/
(kill)https://mixkit.co/free-sound-effects/game/

//**START SCREEN**

For the background image, I've found a pixelated room gif from google. 
Insert image here
For the moving title, I made something similar to the example that was included in the Week 5 Github folder.
For the blinking insruction text, I've used framecount and modulus to make it blink. 
Insert image here

//**ISSUES**
My audios were coming out distorted when I played them. i realized that it happens if I put the audios by themselves within the function or draw function.
I've found the solution from the following link.
https://discourse.processing.org/t/i-am-trying-to-load-in-a-sound-file-to-my-p5-sound-project-but-they-all-come-out-distorted-or-my-screen-goes-black/6121
