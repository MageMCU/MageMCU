# About MageMCU

<p align="center">
	<strong>--- Blinking LED ---</strong>
</p>

The *Hello World* cliche is still blinking... Hello, I'm Jesse. I've been fascinated by the magic of modern tech. My interest is programming the AVR which is a family of microcontrollers (MCU) developed by Atmel, acquired by Microchip.

## The two wheeled differential drive mobile robot

I did put together a rudimentary robot to study the interfacing and programming the MCU. Yet, there are many inexpensive two wheeled differential drive mobile robots (DDMR) on sale. The brains for the DDMR is the most used and popular **Arduino Uno Rev3** board (UNO). 

<p align="center">
	<img src="https://user-images.githubusercontent.com/87388066/192183593-076dc5a1-4fb2-4893-b88e-f223ffb8636a.jpg" width="400" />
</p>

## Atmega328P

At the heart of the **UNO** is the Atmega328P-PU (atmega328p) MCU. The 28-pin DIP package is easily replaced if damaged. Furthermore the **UNO** board with the completely removed atmega328p chip can be used as a programmer.

- [From Arduino to a Microcontroller on a Breadboard](https://docs.arduino.cc/built-in-examples/arduino-isp/ArduinoToBreadboard/)
- See datasheet...

Note that Arduino as ISP for Arduino Bootloaders below clarifies and exemplifies the one described here...

## ATmega16U2 

The ATmega16U2 chip on the Arduino Uno board acts as a bridge between the computer's USB port and the MCU serial port. 

- [Updating the Atmega8U2 and 16U2 on an Uno or Mega2560 Using DFU](https://docs.arduino.cc/retired/hacking/software/DFUProgramming8U2/)
- See datasheet...

## Bootloader

- [Arduino as ISP and Arduino Bootloaders](https://docs.arduino.cc/built-in-examples/arduino-isp/ArduinoISP/)


## AVR Programming

Many beginners use the [Arduino IDE software](https://www.arduino.cc/en/software). The advanced AVR programmers may use the [MS Visual Studio Code](https://code.visualstudio.com/) using the [PlatformIO core](https://platformio.org/). 

- Study the AVR Tool Chain - Essential Guide used for Makefile - [Standard C library for AVR-GCC](https://www.nongnu.org/avr-libc/user-manual/overview.html)

	- [AVRdude Utility](https://github.com/avrdudes/avrdude)

[AVR Professional Programming Software](https://www.microchip.com/en-us/tools-resources/develop/microchip-studio)

## Bare Metal Programming

- [Introduction to Bare Metal AVR Programming](https://www.youtube.com/watch?v=meGMw8K0NGk)
- [Practical Guide to Bare Metal C++](https://arobenko.github.io/bare_metal_cpp/)

## Make utility

- [Using make and writing Makefiles](https://www.gnu.org/software/make/manual/make.html) - When writing a MakeFile that uses avr-gcc, avr-objcopy and avrdude, Google search with the following keywords: **Makefile Atmega328P Github**.

## Programming Language

The procedural **C** prograomming language is used by beginners and then move to object-oriented programming (OOP), the **C++** programming language. 

- Programming: Principles and Practice Using C++, 2nd Edition - [(Pearson - Learning. For life.)](https://www.pearson.com/us/higher-education/program/Stroustrup-Programming-Principles-and-Practice-Using-C-2nd-Edition/PGM270453.html)

	- [Author:](https://www.stroustrup.com/index.html) Bjarne Stroustrup's homepage.
	- [Source:](https://www.stroustrup.com/programming.html) More information on his book, PPP2.
	- [Support for PPP2](https://www.stroustrup.com/programming_support.html) This includes the source code for the book.
 
The reasoning behind the repository publication is to further my studies in the C++ programming language to include C++ templates along with C++ meta programming. Many in the industry would narrow the modern C++ language down by encapsulating it into a singularity called abstraction. Unfortunately, many like myself where the modern C++ abstraction is difficult to grasp.

Second to None is the  [Python Programming Language](https://www.python.org)

## Libraries

- [Arduino Core](https://github.com/arduino/ArduinoCore-avr)
- [Arduino Libraries](https://www.arduino.cc/reference/en/libraries/)
- [PlatformIO Documents](https://docs.platformio.org/en/latest/)
- PlatformIO Project Configuration File [platformio.ini](https://docs.platformio.org/en/latest/projectconf/index.html)
- [PlatformIO Registry](https://registry.platformio.org/)
- MCUdude [MightyCore](https://github.com/MCUdude/MightyCore)

## Lab Notebook: Science - Physics - Chemistry - Engineering - Electronics - Robotics

- Writing the Laboratory Notebook (US Department of Education) - [(PDF file)](https://files.eric.ed.gov/fulltext/ED344734.pdf)
- Laboratory Notebook with permanent numbered pages.
   - Scientific Notebook Company - [(Take a look at an example on lab notebooks)](https://snco.com)

## Electronics Textbook

- Introductory Circuit Analysis author Robert L. Boylestad, 13th and now the new 14th edition
- Laboratory Manual for Introductory Circuit Analysis, 13th edition

## Electronics Courses

- Bad bad physics - from Maxwell's equations to Kirchhoff's Laws - don't fret it's all good - ha ha
	- [MIT OpenCourseWare - Circuits And Electronics](https://ocw.mit.edu/courses/6-002-circuits-and-electronics-spring-2007/)
- Study **Ohm's Laws** while learning how to use the **Multimeter**
	- Say the following five times real fast...
 		- **amps ohms volts**
- [Oscilloscopes 101 for Engineering Students](https://www.youtube.com/playlist?list=PL2XuMA5AwNUznkBE46tcZAF3p5Edxgm-z)

## DIY Beginners Desktop Lab

- [Make a One Desk Electronics Lab](https://www.instructables.com/Make-a-One-Desk-Electronics-Lab-in-a-Small-Place-f/)
- [A DIY electronics lab for beginners](https://thesmarthomejourney.com/2020/10/12/diy-electronics-lab-desk/)
- Please Read the ***MageMCU Disclaimer***
- **Safety Data Sheets**, where to find **MSDS** and **SDS** on the internet... **Safety Comes First**.
	- OSHA Laboratory Safety Guidance [PDF](https://www.osha.gov/sites/default/files/publications/OSHA3404laboratory-safety-guidance.pdf)
	- OSHA Hazard Communication Safety Data Sheets [Quick Card PDF](https://www.osha.gov/sites/default/files/publications/OSHA3493QuickCardSafetyDataSheet.pdf)
	- Pb Lead-Free RoHS Exempt [PDF](https://web.calce.umd.edu/lead-free/SMTAExemptMay8.pdf)
- [Five essential tools for electronics lab safety](https://www.arrow.com/en/research-and-events/articles/five-essential-safety-products-for-every-electronics-lab)
- Parents and Teachers On Safety Transparency
- As a warning, such laboratories at home or at school may catch fire.
	- Recommended Student, Parent and Teacher Signed Agreement
		- Emergency Phone Numbers
		- Home Address
		- Contact Information
		- Legal Permissions for Hospitalization
		- Legal Disclaimer
		- Witness Name & Signature
		- Sign and Date
	- The motivation behind this type of an agreement, there is not enough all-around laboratories in our public schools for vocational readiness. Let's get America back to work.

## Tentative Disclaimer

- This page is meant for the author and belays with the author. If anyone disagrees with its content, please contact the author...
- Jesse Carpenter doing business at Carpenter Software LC - Email Address: carpenter.software.lc@gmail.com

## Disclaimer and Terms

Please follow the ***Disclaimer*** and ***Terms*** in each of the Depositories here at MageMCU.

