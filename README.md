ZorkBound
=========

A short and sweet text adventure written as a CCScript tech demo.

ZorkBound's name is slightly misleading. There are no mazes of twisty little
passages, all alike; you are not at all likely to be eaten by a grue. Instead,
you assume the role of Z. Namelessprotagonist (a tragic mixup with the health
department when issuing the birth certificate; don't ask), a lost soul on a
mysterious journey that begins in an old house and also ends in an old house,
and has some wandering around in an old house in between.

The main purpose of this project was to demonstrate the cool things that could
be expressed in an EB hack, using the CCScript programming language.

The CCScript code contains a lot of neat stuff, not least of which is a custom
item tracking core based on a library that provides simple arrays and linked
lists, written in a MIPS-like DSL implemented with CCScript, which compiles to
EarthBound bytecode, which is interpreted by a VM running on a 65816. And for
all that, the entire system of objects is tracked using only 1024 bytes of
memory! Who ever said abstraction was expensive?

(Well, actually it is: the doubly-interpreted system is noticeably slow when
run at native Super Nintendo clock speeds... but I digress.)


How to build
============

1. Use a recent version of Visual CCS, available here:
     http://starmen.net/pkhack/ccscript

2. Take an unedited EarthBound ROM (with header), expanded to 32 megabits, and
   apply Base.ips to it. Base.ips contains EB++ 0.6, along with some custom
   window graphics and a few other tweaks.

3. Load ZorkBound.pkproj in Visual CCS and hit "Compile!"

