I've worked on a number of demos now, learning all sorts of different things: parallax scrolling, progen scenes, unrolling LDIRs blitting, sprites, border effects, user input, stack blitting, self-modifying code, floating bus tricks...

Now it's time to pull it all together and create a game. In theory I have all the building blocks so this will be simple right? Well experience tells me that the devil will be in the details, so I'm sure I'll learn lots still as I manage multiple screens, manage game state, collision detection, etc, alongside all my cool border tricks and stack rendering. 

I'm also planning to learn some more optimizations. Each demo I found new tricks. The main trick for this demo is using (HL) more. INC (HL) is 11T vs LD A, (HL)/INC A/LA (HL), A. And JP (HL) is faster than a label: no wonder people always talk about jump tables! 

tl;dr concept of game: our protagonist falls down a hole, and must get to the bottom in time without dying to save an elf. 

Terrible idea for a game: but it gives us a hole to fall down. And procen bg and obstacles. And stack-based scrolling - hopefully 18-col wide hole using IX/IY registers as well for stack render! 
Game status shown in top border, leaving sides of main screen to shw distance to bottom of whole. ANd other border tricks on title screen and the like. 

