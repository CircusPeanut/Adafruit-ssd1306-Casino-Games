# Peanuts Slot Machine

Hello!  This is the code for a simple, three reel video slot which is exculsivly meant for the Adafruit ssd1306 32x128 i2c OLED display.

It requires 

1x Adafruit ssd1306 32x128 i2c
1x Joystick
1x Microcontroller
1x Pushbutton
1x RGB LED
Wires and so forth..

The code works by listening and waiting for the Joystick knob to be held down.  There is a starting balance integer as well is a "bet level" integer. 
When the proper value is met, a suqence of events that decides the symbol on each reel begins.  The reels and their respective 
corrisponding values are all labled A B and C from left to right.  A number between 1 and 20 is randomly
chosen, and then a score counter for the win id is kept for that reel, and then the same happens for the
next reel, and the next.  When all three symbols are chosen, a long list of "if" checks occur, looking for winning combinations, and then the bet level is multiplied by a set amount and added to the balance if a win is found.
I would love help in shortening and abreviating the winning sequences with "or" logic for the wild symbol.  I had to make a sperate
"if" check for each possible configuration of wilds, using a lot of the Nanos memory.
