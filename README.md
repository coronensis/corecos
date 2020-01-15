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

Do you remember this:

![C64](C64.gif  "Animated C64 startup screen")

?

If you do not, you may want to read up on the good old [Commodore 64](https://en.wikipedia.org/wiki/Commodore_64), a venerable
8-bit-era home computer.

Now imagine having something that looks and feels like the C64 but uses modern
hardware with many times the processing power, memory space and external
storage than what the original could offer, but still keeps the flair of a traditional 8-bit system.

The intended usage of the system is for building and running simple retro-style games.

I am considering the following configuration:

- "Modern" 32-bit RISC CPU clocked at ~25 MHz instead of the 6502 clocked at ~1MHz.
I am currently implementing a simple RISC-V RV32I core, good enough to run this system.
See [Rival](https://github.com/coronensis/rival) for details.

- 1 MB of RAM instead of 64 KB.  With some KB of fast CPU internal RAM.

- 1 GB microSD card instead of the Tape or Floppy drive

- PS/2 keyboard interface

- Homebrew sound interface (a resistor ladder)

- VGA 320 x 200 resolution display interface in 8 colors (instead of 16)

- Built-in machine monitor (instead of one on a cartridge)

- UART for background debugging and access to the machine monitor

- "C" language interpreter instead of the BASIC interpreter

- Simple operating system. User interface similar to the old Basic interpreter

- Library with some common primitives for access to OS, screen, keyboard,  etc.

Implementation will happen around an FPGA and the constraints given are determined by
what my FPGA development board (an "ancient" Spartan 3 Starter Board) has to offer.

As for the naming: The project has nothing to do with Corona Data Systems (Cordata)
but makes a reference to project's place of birth . Corona is one of the historical names of
the city of Brasov in Romania.

This project is a tribute to [CoBra](http://cobrasov.com/CoBra%20Project/index.html).

