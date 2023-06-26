A library for use the board with Microsoft Bascom (Basic compiler) and Fortran-80.
I have test it under CPM 2.2.

Usage :

1_ compile library sources (after adjusting the FPU address into am9511.mac)

"m80 = am9511.mac/L" --> am9511.rel

"m80 =apu.mac/L" --> apu.rel

The address to use depend of the slot you use into the Apple II.
I have use slot 1.
Be careful that address are not the same in 6502 mode and in Z80 mode.

2_ create the library

"lib80 libapu.rel=am9511.rel,apu.rel/e" --> libapu.rel

3_ compile a basic test program

"bascom =btest.bas/o/l" --> btest.rel

4 link with or without the library (for use ou not the fpu)

(with) "l80 btest.rel,libapu.rel,aputst.com/n/y/e"

or (without) "l80 btest.rel,aputst.com/n/y/e" --> btest.com

There is some warnings about double definitions but works well...

Inspired for the job of ratboy666 here : https://github.com/ratboy666/apu
