This is information about a FPU board I made for my Apple IIe.

I do that because I want one usable with DOS 3.3 and with CPM + Z80 Softcard.

They use AMD AM9511 / Intel C8231.

If you dont use interrupt (I mean if you dont have a routine that manage the interrupt) leave the INT J2 jumper open.

J4 must be put to GND (as on the picture).

The board can be set for 4 MHz clock or 2 MHz clock (J3 jumper).
Usually AMD --> 2 MHz, INTEL --> 4 MHz but double check the exact reference of your FPU. 

Have fun !

20/06/2023
Philippe Roehr
