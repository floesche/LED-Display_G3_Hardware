---
title: Arenas
parent: Generation 3
nav_order: 3
---

# Recommended method for assembling arenas

## Assembling the LED matrix.

The standard arena consists of a circular array of 8x8 dot matrix displays of LEDs connected to microcontrollers in a 1:1 manner. The typical 12 panel ring arena is built from two PCB boards, and is typically 4 panels high (48 panels total). In order to later control the displays, unique addresses must be assigned to each one. These microcontrollers may need to be flashed with the latest files according to the quick start guide on the panels wiki ([[https://bitbucket.org/mreiser/panels/wiki/Home | Home]]) before assigning addresses. The following outlines the steps needed for creating a standard arena with a 4x11 array of LED displays.

1. Press each LED display into the microcontroller using the correct orientation. With the male side of the controller pointing down, the ink stamp of the LED should be on the right hand side before inserting pins.
1. Once 44 microcontroller/LED units have been assembled (or more, if some microcontrollers are not functioning), they must first be programmed and assigned addresses as outlined in the [[https://bitbucket.org/mreiser/panels/wiki/Quick_Start | Quick Start guide]].
    1. If the LED does not properly display lights, or is very dim compared to the rest, do not use it in your arena.
1. Connect each column to form the 12 columns of the matrix above. This will probably require partially pulling out the LED portion of each unit, connecting the male and female ends, and then securing the LED to the microcontroller once the connection is snug. (Note this problem may make itself more apparent when viewing the assembled columns, and fixing it will ensure strong electrical connections between units).


## Assembling the boards.

The PCB boards for each arena require some soldering. Remember both boards must be facing up in the final arena, attach components on the correct side.

1. Bottom board (female end) requires 12, 8-pin stacking headers soldered around the center top (silkscreen text) circle cutout  side of the board.
1. Bottom board requires 4 capacitors, one in each corner of the board, with the correct polar orientation (see board, light stripe to the left).
1. Bottom board also requires a power supply input, jumpering pins, a switch, serial port, and switch to be securely soldered.
1. The top PCB should have male headers soldered to the bottom side (opposite the silkscreen text) that fit into the connectors of the top panels (additional components are not required on the top PCB, but capacitors are always a good idea). 
1. Connect the LED columns to the bottom, then top boards.
1. Check that the panels turn on and are in the correct place by plugging in the 5V power supply and turning on the arena with the power switch.
1. Check for gaps between LED panels which can compromise the long term stability of the arena.

![An assembled arena - top view](https://github.com/reiserlab/Panel-G3-Hardware/blob/master/resources/arena_top1.jpg)
![An assembled arena - side view](https://github.com/reiserlab/Panel-G3-Hardware/blob/master/resources/arena_side1.jpg)

## Constructing the Arena Housing:

Our lab uses supplies from [Thorlabs](http://www.thorlabs.com/) to construct a holder for the arena, IR diode, IR sensor, tether post, and camera. This can be accomplished with any sturdy materials, although Thor components are recommended because of their high modularity and strength (and labsnacks). Instead of giving exact directions, some required specifications will be listed.

1. The IR diode must be positioned pointing directly down on the center of the arena.
1. The IR sensor must be positioned directly under the center of the arena.
1. The tether post must end in the exact center of the arena with the fly between the IR diode and sensor, and at an 20-35 degree angle to the perpendicular.
1. The most useful placement of a camera is level with the fly for alignment purposes. 

## Connecting Components:

The assembled arena and remaining components must be properly connected using mainly BNC, USB and Serial Port connectors. When setting up the rest of the system, place all components in a user friendly arrangement (i.e. oscilloscope and analog camera output easily viewable). The following is a table, then diagram of connectivity. For more information on how each component works, see the “Flight Simulator User Guide”  by Frye, Reiser, and Dickinson or read the Panels documentation page.

The following is a list of Components and connections in the format:
Component   **Connection**	*Connection(s)*	 (i.e. the first line reads: the controller's ADCO is connected to the Wing beat analyzer's WBA input)

Controller	**ADC0**	*WBA L*

Controller	**ADC1**	*WBA R*

Controller	**DAC0**	*Nidaq Input 3*

Controller	**DAC1**        *Nidaq Input 4*

Controller	**PC1	** *Serial Port to PC*

Controller	**I2C	** *Serial Port to Arena*

Nidaq 	**Analog Input 0** *Wingbeat Amplitude L*

Nidaq	**Analog Input 1** *Wingbeat Amplitude R*

Nidaq	**Analog Input 2** *WBA Frequency*

Nidaq	**Analog Input 3** *Controller DAQ1*

Nidaq	**Analog Input 4** *Controller DAQ2*

Nidaq	**Analog Input 5** *Wingbeat Amplitude L-R*

Nidaq	**Analog Input 6** *Analog Output 1*

Nidaq	**USB Output** *PC*

Nidaq	**Analog Output 1** *Analog Input 6*

Wingbeat Analyzer	**WBA L** *Controller ADC0, Nidaq AI 0*

Wingbeat Analyzer	**WBA R** *Controller ADC1, Nidaq AI 1*

Wingbeat Analyzer	**Signal Out L** *Oscilloscope Ch 1, Speakers*

Wingbeat Analyzer	**Signal Out R** *Oscilloscope Ch 2, Speakers*

Wingbeat Analyzer	**WBA L-R**	Oscilloscope *Ch 3, Nidaq AI 5*

Wingbeat Analyzer	**SYNC (-TTL)** *Oscilloscope Ext Trig*

Wingbeat Analyzer	**LED Out** *IR LED on Flight Arena*

Wingbeat Analyzer	**Photo detector** *Photo detector on Flight Arena*

Wingbeat Analyzer	**Frequency** *Nidaq AI 2*

Oscilloscope	**Channel 1** *WBA L*

Oscilloscope	**Channel 2** *WBA R*

Oscilloscope	**Channel 3** *WBA L-R*

Oscilloscope	**Ext Trig** *WBA SYNC (-TTL)*

Flight Arena	**Serial Port** *Controller I2C*

Flight Arena	**Photodetector** *WBA Photodetector*

Flight Arena	**LED** *WBA LED Out*

PC	**USB** *Nidaq*

PC	**Serial Port** *Controller PC1*

# Power issues

(needed)