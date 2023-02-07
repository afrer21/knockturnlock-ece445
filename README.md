# knockturnlock-ece445
Team Members:
- Jack Kelly (jacktk2)
- Vishal Rajesh (vrajesh2)
- Adam Frerichs (adamdf2)

Link to high-level block diagram: https://docs.google.com/document/d/1kzdScCKG7YJrnN6E_D_-xf1Sez1VTvAVJpIW24HritI/edit?usp=sharing

# Problem

Losing keys is extremely common, and being locked out of your own house can be extremely frustrating. Hidden spare keys are a security concern, and digital keypads can be unsightly as well as insecure, introducing a secondary point of failure to possible intruders.

# Solution

Describe your design at a high-level, how it solves the problem, and introduce the subsystems of your project.

We propose a unique door lock, that uses a unique combination of programmable knocks and door knob turns in order to provide a secondary way of unlocking a door. From an outside observer, it would simply appear as somebody let the entrant inside, after they knocked and tried the handle, and would not have any obvious code for potential intruders to figure out. It would consist of a sensor to detect knocks, two buttons to read left and right knob turns, a microprocessor to check for the specific code, and a usb-port hidden in the side of the door in order to program a new combination.

# Solution Components

## Piezo sensor

These sensors are able to detect vibration due to knocking, and are used in things like electric drum kits to detect the percussion.

When activated through a force, piezo sensors are modeled as a capacitor. This would be connected to the microcontroller using a transistor in order to produce a binary output, and connected to a ground through a small value resistor, in order to allow the voltage to discharge quickly and have knocks be processed in quick succession.

## Button

The buttons would have to have low spring resistance, in order to make the knob feel like a regular locked door handle. These would be connected to a high voltage source with a pull-up resistor in order to produce a binary output, with one button on both the left and right sides of the door knob mechanism to detect both directions.

## Microcontroller

https://www.snapeda.com/parts/STM32F103C8T6/STMicroelectronics/view-part/

This is the microcontroller the RFID lock group used. It may be more complex than we need.

This would be mounted on our PCB, which would need to fit in an enclosure less than 2” thick in order to fit in the door. However, it could be as wide as needed as long as it fits inside of the door.

## Power

The device would be powered directly through the house’s power, and would require a 3.6V AC/DC converter in order to match the input power of the microcontroller. The electronic lock would require 9V AC/DC converter. These would be separate from the PCB enclosure, and as such would have to be less than 2” in thickness in order to fit within the door.

## Electronic Lock

https://www.adafruit.com/product/1512?gclid=Cj0KCQiA2-2eBhClARIsAGLQ2RlgWKqt1XGgX23roDPViY1hjU2EkBonYtzCMKPVEfRFaTNxiRkg-D8aAtL6EALw_wcB

This lock would be sufficient for the project as we would not need to design our own lock and servo system. When a correct combination is entered the microcontroller would send a signal to unlock the door and then the lock would re engage when the door closes.

# Criterion For Success

Describe high-level goals that your project needs to achieve to be effective. These goals need to be clearly testable and not subjective.

The code must be inputtable consistently by an authorized user, but precise enough to avoid random entrance.

The lock needs to be easily programmable in order to change the combination.

The knock/vibration sensor needs to be sensitive enough to detect quieter knocks, but not be triggered by regular activities like walking around an apartment.

The knock combination needs to be rhythm based, in order to mimic a regular knocking pattern.
