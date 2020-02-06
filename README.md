# Lightweight Multitasking Executive (LMX)

Suitable for Robotics using Embedded Processors.

A real-time lightweight multitasking executive is implemented by the code in "task.cpp" file.  It uses a linked list of data structures and stacks to allow real-time cooperative tasks to run round-robin in parallel.

This works in conjunction with a 1kHz system 'sysclock' timer, provided by the companion code in "sysclock.cpp" and "sysclock.h", to implement millisecond timed delays and periodic execution.

To build the LMX library, edit "task.h" and set **MACHINE** to the required architecture. Currently that's:

* **MACH_M68K** MC68332  MiniRoboMinds 332
* **MACH_AVR** Mega2560, Mega328, Teensy-LC
* **MACH_ARM** Teensy3.1

Note that the AVR and ARM builds assume the Arduino IDE with the Teensy plugin.

by [David P. Anderson](http://www.geology.smu.edu/~dpa-www/myrobots.html) and [DPRG](https://www.dprg.org/)
