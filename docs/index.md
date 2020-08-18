---
title: Hardware
parent: Generation 3
has_children: true
nav_order: 1
---

# Home

These pages document the hardware details of the controller project (PDC 3.0, released April 2011). The documentation for the version 2 of the project is archived [here](../../Software/docs/g2-panels.md).

What is new in PDC 3.0?

- Xmega controller
- 4 I²C busses
- improved ADC and DCA components

# At a Glance

1. The flight arena consists of a circular array of 8x8 dot matrix displays of LEDs with additional electronics to drive the display.    
1. The data acquisition module is often called the nidaq, or National Instruments Data Acquisition Device. In this case, the nidaq is a NI USB-6229 BNC Multifunction DAQ. This model has 16 analog inputs, 4 analog outputs, 8 DIOs and 2 user defined BNC terminals—more information about this device is available at http://sine.ni.com/nips/cds/view/p/lang/en/nid/203866.
1. The controller is a microprocessor circuit custom designed to operate the flight arena. The controller communicates with a PC through a serial port and to the panels using a rapid serial interface. 
1. The wingbeat analyzer measures the frequency and amplitude of the fly wing stroke. It also computes the sum and difference of the amplitudes of the left and right wings. This device is custom built by JFI Electronics at the University of Chicago.
1. The PC is used to display patterns on the flight arena and record data through the nidaq. The PC must be capable of running Matlab as well as a data acquisition program such as AxoScope or Spikehound. It must have at least one USB and one serial port.
1. An oscilloscope with three input channels and an external trigger will suffice. 

# Required parts

The following is a brief list of the parts needed for a functional setup.

## Data Processing & Acquisition

1. Arena Controller -  (URL/controller details neeeded)
1. Wingbeat Analyzer (WBA) - [JFI Electronics Laboratory](https://jfi.uchicago.edu/), University of Chicago.
1. Data Acquisition Module -  [National Instruments Data Acquisition PCI-6221 Board (NIDAQ)](http://sine.ni.com/nips/cds/view/p/lang/en/nid/14132)
1. Oscilloscope - [Tektronix TDS 2024B](https://www.tek.com/products/oscilloscopes/tds2000/)
1. PC - Any PC capable of running matlab, a data aquisition program, and handling the card drivers for the NIDAQ. - Our setup uses Dell Precision T5500
1. Cables - BNC, BNC-Bannana adaptors, BNC T splitters, Firewire, USB A-B

## Flight Arena & Peripherals

(See [Arenas Page](arenas.md) for assembly information)

1. [LED Display Panels](../../Software/assets/Green%20Panels%20BM-10288MD.pdf)
1. Arena Boards  -  (needed)
1. IR Sensor/Cover  - (needed)
1. IR Diode - (needed)
1. Camera    Point Gray Research [Firefly](http://www.ptgrey.com/products/fireflymv/fireflymv_usb_firewire_cmos_camera.asp)
1. Stage  -  [Thorlabs](http://www.thorlabs.com) components 
1. Enclosure  -  Any material capable of covering the arena and preventing light from entering.
1. SDHC/CF Card  -  Such as from  [Transcend](http://ec.transcendusa.com/product/product_memory.asp?Cid=92)

## Software

1. [Matlab](http://www.mathworks.com/products/matlab/)
1. Data Acquisition  -  Such as [Spikehound](http://spikehound.sourceforge.net/) or the Matlab Data Acquisition Toolbox


## Optional

1. Speakers - To hear the WBA
1. 80mm PC Case Fan  -  To encourage fly flight
1. Thermometer - For temperature sensitive experiments/consistency.