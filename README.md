# CISCComputerSimulator
## CISC Simulator - Team 1
A CISC Simulator was developed using JAVA (JDK version 19).
Refer to Design_Document.pdf for more information.

## Preparation Instructions
### Prepare Environment for execution
NOTE: Please make sure your system is running on JDK version "^19".

## Start Execution
Once the files are extracted from the zip folder, double-click on the CISCComputerSimulator.jar file.
Or
To run the project from the command line, go to the dist folder path and type the following: java -jar "CISCComputerSimulator.jar"

## Operation of the Simulator
### How to IPL
Clicking on the "IPL" button will take the IPL.txt file from the unzipped location.
Clicking on the "Custom IPL" button will open a Dialog box to select the IPL file that the user wants to select (It doesn't necessarily have to be named IPL.txt)
Starting location where the simulator executes code
Once the "IPL" button or "Custom IPL" is clicked, the first location mentioned in the first line of the txt file would be taken as the PC.
For eg. If the IPL.txt contains the below content:
0006 004F
000A 0009
0020 000A
The PC would have the value 0x0006
### How to Single Step
Clicking either "IPL" or "Custom IPL" will load the PC with the first memory address location, then Click on the "SS" button to Single Step.
or
If memory values have been manually stored, Load the PC value with the memory that needs to be Single Stepped, and then Click on the "SS" button.
How to Run the machine code
Clicking either "IPL" or "Custom IPL" will load the PC with the first memory location, then Click on the "Run" button to Run the machine till it Halt instruction is encountered.
or
If memory values have been manually stored, Load the PC value with the memory address from where the instruction should be run, and then Click on "Run" button.
Note: When Halt is encountered, HALT Led would glow up and the machine would stop.
### How to read memory locations
Click on the Instruction toggle bits corresponding to the memory address and Click on LD corresponding to MAR.
Click on the "Load" button, and MBR will be loaded with the value/instruction stored in MAR.
### How to store memory
Click on the Instruction toggle bits corresponding to the memory address and Click on LD corresponding to MAR.
Click on the Instruction toggle bits corresponding to the value/instruction and Click on LD corresponding to MBR.
Click on the "Store" button, MAR will be stored with the value/instruction stored in MBR.
Clicking on "Store+" instead of "Store" will do the same operation as Store, in addition to that it'll also increment the MAR.

### How to execute Program 1
Click on the “Load Program 1” button then the PC will be loaded with starting address, Click on the “Run” button
Program 1 execution will be started 
Whenever the Input LED glows, Enter one digit from the keyboard, and wait for the Input LED to glow to enter the next digit or to press enter(signalling the end of that number input).
The corresponding entered input will be displayed in the printer
After entering 21 numbers, the Closest value to the last entered input will be displayed on the printer. 

### How to execute program 2
Click on the “Load Program 2” button to load the content of Program2_text.txt into memory and load the instruction list from Program2.txt. 
Once the “Run” button is clicked, the printer will first print the content of the paragraph character by character, once the content is printed it will prompt the user to enter the word to be searched.
Whenever the Input LED glows, enter one character in the keyboard, and wait for the Input LED to glow to enter the next character or to press enter (signaling the end of that word input).
The corresponding word will be printed on the printer as well.
The program will then go on the check if the word is present or not in the paragraph, if it exists it will print “Word found!” and print the Line # and Word # where it was found, or else it will print “Word not found”. 
