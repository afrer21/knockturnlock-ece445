# Adam Frerichs' ECE 445 Lab Notebook
Photos of the project are in the pics folder off the main folder
## 2/22/2023
### Objectives:
- Finalize part requirements
- Order first round of parts
- Finish design document
### Completed:
- Still finalizing part requirements
- Ordered first round of parts, still need to order microcontroller and voltage regulator
- Decided on using a 1M ohm resistor for the piezo as research has told us the larger the resistor the lower the voltage readings we will get. A 1M ohm resistor should get us readings within the 5V threshold that we want
- Completed design document

- Below is the reference sheet for the microcontroller we decided to use
[9] Atmel 8-bit AVR Microcontroller with 2/4/8K Bytes In-System Programmable Flash, Atmel. August 2013. [Online] Available: https://ww1.microchip.com/downloads/en/DeviceDoc/Atmel-2586-AVR-8-bit-Microcontroller-ATtiny25-ATtiny45-ATtiny85_Datasheet.pdf

## 2/23/2023
### Completed:
- Submitted design document
- Signed up for design review

## 2/24/2023
### Objectives:
- Meet with TA
- Complete team contract
### Completed:
- TA says we are still on track
- Submitted team contract
- I have been tasked with mainly working on the microcontroller section and Arduino programming

## 2/26/2023
### Objectives:
- Review design document
### Completed:
- Reviewed design document

## 2/27/2023
### Completed:
- Design review
- Need to fix requirements and verification tables with more actionable verifications

## 3/1/2023
### Objectives:
- Peer design review
- Begin schematic
- Finalize part requirements
### Completed:
- Attended and submitted peer design review
- First draft of schematic
- Parts not yet ordered should all be able to be obtained in the ECE services shop

## 3/5/2023
### Objectives:
- Finalize schematic
- Revise design document
### Completed:
- I still need Jack and Vishal to look over the schematic and then we need to actually route and place everything on the physical PCB
- Improved the requirements and verification and the other small suggestions by Vishal (TA)

## 3/6/2023
### Objectives:
- Submit PCB order
### Completed:
- Made slight modifications to PCB design in order to pass review for submission
- PCB was missing once connection to ground that the review was able to catch
- Gerber received by Jason (TA)

## 3/7/2023
### Completed:
- Submitted teamwork evaluation

## 3/9/2023
### Objectives:
- Discuss with team what needs to be worked on over spring break
### Completed:
- Decided we need to start our software program and finish it before the PCB arrives
- Need to collect all of our components when we come back from break

## 3/22/2023
### Objectives:
- Meet with TA
### Completed:
- Picked up ordered parts from the lab
- TA says we are still on track on should keep continuing as we have been

## 3/23/2023
### Objectives:
- Outline software program
### Completed:
- Created rough outline for software program

## 3/27/2023
### Objectives:
- Begin converting software outline to code
### Completed:
- Some of the software program is written, have not been able to unit test any of it so far

## 3/28/2023
### Objectives:
- Start individual progress report

## 3/29/2023
### Completed:
- Finished individual progress report

## 4/3/2023
### Objectives:
- Continue writing code for software program
### Completed:
- Basic software program has been written, still have not been able to test any of it

## 4/4/2023
### Objectives:
- Continue writing more advance features of software
### Completed:
- Continued writing more advance features of software, still no testing

## 4/6/2023
### Objectives:
- Solder and test first PCB
### Completed:
- Picked up small parts for soldering
- Ordered more components for our project, ordered more ATtiny85s with different footprints in case our second PCB did not come in on time
- Ordered a revised PCB, we need to fix one routing that was missed on the schematic for the microcontroller, the footprint for the microcontroller was wrong

## 4/13/2023
### Objectives:
- Solder and test PCB
### Completed:
- Used stencil to solder on surface mounted components
- Had no access to a program loader so we decided to wait and finish soldering

## 4/14/2023
### Objectives:
- Finish solder and test PCB
- Meet with TA
- Build the board
### Completed:
- Finished soldering all components to board
- Agreed upon with TA a time to mock demo, April 20th 4:00 PM
- Finished building the board
- Decided to ditch the programming circuit we had designed and instead added an IC socket for the microcontroller. This would allow us to program the ATtiny85 separately on our program loader, then just directly place the pre-programmed microcontroller onto the PCB. This actually worked well and solved our issue of not being able to program

- The image below shows the front of the project
![front of project](https://github.com/afrer21/knockturnlock-ece445/blob/main/pics/Exterior.JPG?raw=true)

## 4/19/2023
### Objectives:
- Write test program for mock demo
- Get hardware ready for mock demo
### Completed:
- All ready for mock demo
- We have unit tests running for the mock demo that allow the TA to see that each of our subsystems is running and that we only need to continue improving the software
- The unit tests flash an LED to show that the microcontroller has received a handle turn or a knock

## 4/20/2023
### Objectives:
- Finish writing software program
- Finish connecting all sensors
### Completed:
- Mock demo
- Software and hardware all functioning as expected
- We added software that allows us to reprogram the combination on the fly. We were originally keeping that idea as something we could add in the future, but we had extra time and it was not super difficult to add that portion
- We were having issues with recognizing a knock when it was supposed to be a handle turn. We solved this in software by checking to make sure that the user had not pressed the button when a knock was recorded
- The program is all written and works as expected, we have no current issues with the project and it all works
- We tested the default combination and the reprogramming steps. Demoing the two of these and showing them our project covers all of our high level requirements

- The image below details the back of the project when it is all assembled. You can see that we had to use wires as contact pads, which was not the ideal solution to the problem. The wires ended up working great with the only downside is they look trashy
![back of project](https://github.com/afrer21/knockturnlock-ece445/blob/main/pics/Interior.JPG?raw=true)

## 4/24/2023
### Completed:
- Demo, it went as expected and did not have any issues

## 4/26/2023
### Objectives:
- Start presentation

## 4/27/2023
### Objectives:
- Finish presentation

## 4/28/2023
### Objectives:
- Revise presentation
### Completed:
- Mock Presentation
- Needed to add slide numbers and some more highlighting to important areas on the presentation

## 5/1/2023
### Completed:
- Final presentation, it went as expected and did not have any issues

## 5/2/2023
### Completed:
- Start final paper

## 5/3/2023
### Completed:
- Finished final paper
