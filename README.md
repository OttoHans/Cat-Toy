# Cat-Toy
Programmable cat toy made with a laser pointer and two servo motors.

The idea for the cat toy is to have a randomly moving laser pointer.
The laser pointer will stay within a predefined area defined by four
corners that you program yourself.

Take a square on a graph starting at (0,0), that goes to (180, 180).
That is where the laser pointer lives. These coordinates correspond
directly with the servo motor angles. There are four quadrants to
the square: A, B, C, and D.

A goes from (0, 90) to (90, 180)

B goes from (0, 0) to (90, 90)

C goes from (90, 0) to (180, 90)

D goes from (90, 90) to (180, 180)

In short, it starts at the top left,

then goes down, then right, then up.

There are four corners: cornerA, cornerB, cornerC, and cornerD.
Each resides in its own quadrant.
*each quadrant is held 1 unit away from its respective boarders to
prevent any glitches with servers and programming*
(example, the upper and lower bounds for cornerA is actually
91 to 179)

When programming, you go through each corner and set the location of
that corner by first setting its left/right location, then its
up/down location. Then when you are done, those locations are saved
to EEPROM.
