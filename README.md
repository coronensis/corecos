#  - Work in progress -
Project under construction.


## Overview

```
_________       __________       _________         _________
\_   ___ \  ____\______   \ ____ \_   ___ \  ____ /   _____/
/    \  \/ /  _ \|       _// __ \/    \  \/ /  _ \\_____  \
\     \___(  <_> )    |   \  ___/\     \___(  <_> )        \
 \______  /\____/|____|_  /\___  >\______  /\____/_______  /
        \/              \/     \/        \/              \/

               - Corona Retro-Style Computer System -

```

Remember this:

![C64](C64.gif  "Animated C64 startup screen")

?

If you do not, you may want to read up on the good old [Commodore 64](https://en.wikipedia.org/wiki/Commodore_64), a venerable
8-bit era home computer.

Now imagine having something that looks and feels like the C64 but uses modern
hardware with many times the processing power, memory space and external
storage than what the original could offer but still keeps the flair of a traditional 8-bit system.

The intended usage of the system is for building and running simple retro-style games.

I'm considering the following configuration:

- "Modern" 32-bit RISC CPU clocked at ~25 MHz Instead of the 6502 clocked at ~1MHz.
If I find a small Risc V core I will use it, otherwise a MIPS I R3K will do nicely i.e
the Plasma CPU

- 1 MB of RAM instead  of 64 KB.  With some 16 Kb of fast CPU internal RAM.

- 1 GB microSD card instead of the Tape or Floppy drive

- PS/2 keyboard interface

- Homebrew sound interface (resistor ladder)

- VGA 320 x 200 resolution display interface in 8 colors (instead of 16)

- UART for background debugging and access to the machine monitor

- A built-in machine monitor (instead of one on a cartridge)

- A C interpreter instead of the Basic interpreter

- Simple operating system. User interface similar to the old Basic interpreter

- Small library with some common primitives for access to OS, screen, keyboard,  etc.

Implementation will happen around an FPGA and the constrains given are
determined by what my FPGA development board (a Spartan 3 Starter Board) has to offer.

Most of the components needed will be sourced from other open source projects, be it
HDL or C source code. My contribution will be to find the right stuff and "glue"
it all together, implementing whatever there will missing in the end.

As for the naming: The project has nothing to do with Corona Data Systems (Cordata)
but makes a reference to project's "birth"place. Corona is one of the historical names for
the city of Brasov in Romania.

This project is a tribute to [CoBra](http://cobrasov.com/CoBra%20Project/index.html).

