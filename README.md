Marlin-Shapeoko-CNC
===================

Excerp:
-------
This code is almost the same as the original marlin code, but it has some features, added, removed or tweaked.
This code is tailored to be used with an Shapeoko CNC router. This code should work out of the box with the folling hardware:
 - Arduino Mega (AtMega 1280)
 - RAMPS 1.4 Shield
 - DRV8825 stepper motor driver carrier, high current
 - Active low (optical) endstops
 - Smart 2004 LCD screen
 
Main features adjusted from original:
-------------------------------------
Corrected code to 1/32 microstepping drivers. (correct dimentions and feedrates now)
Temperature controlling code partially disabled.
Power-outputs connected to fan-control (1 fan) and spindle control (2 spindles)
Added M3 (spindle-on) and M5 (spindle-off) commands:
examples:
 - M3 P1 S127  = spindle 1 at 50% duty cycle
 - M3 S255      = spindle 2 (default) at 100% dutycycle
 - M5             = all spindles OFF
 - M5 P2         = Only turn off spindle 2

To-do:
------

 - Fix problems with spindle 1. (some other piece of code is controlling that pin).
 - Change data printed on LCD screen to relevant CNC data.

 
 
 
---------------------------------------------
ELECTRONICS::lab Marlin code for Shapeoko CNC
