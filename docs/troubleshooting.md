---
title: Troubleshooting
parent: Generation 3
nav_order: 4
---

# Tips & Tricks

The [Flight Arena User Guide](https://github.com/reiserlab/Panel-G3-Software/blob/master/resources/flight_simulator_user_guide3.doc) has many suggestions for proper technique.

Some common problems that come up are:

## The Oscilloscope is not showing wing beat waveforms correctly. 

First make sure the fly is directly aligned under the IR LED and above the IR sensor, that the correct BNC cords are plugged in, and that they are the channels shown on the display. The settings commonly used per channel are:
1. 1 V Vertical Scale
1. 2.5 ms Horizontal Scale
1. DC coupling
1. Default (1x) probe voltage
1. Set the trigger to either of the channels with wing beat amplitude or use the TTL from the wingbeat analyzer

Depending on your model, you may need to invert the signals to show the traditional hutchen shape.

If switching settings does not work, try to realign the fly again. 

## A single panel not refreshing correctly 

This means, it stays off, on, or static when a pattern is passed to the arena. If simply resetting the panel and controller do not fix the issue try the following list. A good way to check for functionality is asking the panel controller to display bus numbers (through PControl: Panel > Show Bus Number). If the panel does not update, try the following:

- Turning off the controller, and arena followed by a resetting of the panel, or jiggling in the top and bottom portions to make a snug connection and trying again.
- Reassigning the arena configuration. After placing an arena config file on an SD card using PControl: Configurations > load config to SD card, insert the SD card and set the new config (or old config if you are simply resetting it). To do this use PControl: Configurations > set arena config.
- If the above does not work, you may need to assemble, flash, and address a new panel. 

## An entire column of panels is not turning on.

The likely solution is a soldering issue, if you find the problem is limited to just the one column (i.e. not an issue with the panels) you may need to take the arena apart and re-solder the bottom and/or top PCB boards. Note that the arena does not require the top board to function, but it may aid in stability and establishing solid electrical connections. 