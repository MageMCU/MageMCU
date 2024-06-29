# About MageMCU

<p align="center">
	<strong>--- Blinking LED ---</strong>
</p>

I'm Jesse. I've been fascinated by the magic of modern tech. My interest is programming the AVR which is a family of microcontrollers (MCU) developed by Atmel, acquired by Microchip.

## The two wheeled differential drive mobile robot

I did put together a rudimentary robot to study the interfacing and programming the MCU. Yet, there are many inexpensive two wheeled differential drive mobile robots (DDMR) on sale. The brains for the DDMR is the **Arduino Uno Rev3** board (UNO). 

<p align="center">
	<img src="https://user-images.githubusercontent.com/87388066/192183593-076dc5a1-4fb2-4893-b88e-f223ffb8636a.jpg" width="400" />
</p>

## Atmega328P

At the heart of the **UNO** is the Atmega328P-PU (atmega328p) MCU. The 28-pin DIP package is easily replaced if damaged. Furthermore the **UNO** with a removed atmega328p can bu used as a programmer.

- [From Arduino to a Microcontroller on a Breadboard](https://docs.arduino.cc/built-in-examples/arduino-isp/ArduinoToBreadboard/)
- See datasheet...

## ATmega16U2 

The ATmega16U2 chip on the Arduino Uno board acts as a bridge between the computer's USB port and the MCU serial port. 

- [Updating the Atmega8U2 and 16U2 on an Uno or Mega2560 Using DFU](https://docs.arduino.cc/retired/hacking/software/DFUProgramming8U2/)
- See datasheet...

## Bootloader

- [Arduino as ISP and Arduino Bootloaders](https://docs.arduino.cc/built-in-examples/arduino-isp/ArduinoISP/)


## AVR Programming

Many beginners use the [Arduino IDE software](https://www.arduino.cc/en/software). The advanced AVR programmers may use the [MS Visual Studio Code](https://code.visualstudio.com/) using the [PlatformIO core](https://platformio.org/). 

[Standard C library for AVR-GCC](https://www.nongnu.org/avr-libc/user-manual/overview.html)

## Make utility

- [Using make and writing Makefiles](https://www.gnu.org/software/make/manual/make.html) - When writing a MakeFile that uses avr-gcc, avr-objcopy and avrdude, Google search with the following keywords: **Makefile Atmega328P Github**.

## Programming Language

The procedural **C** prograomming language is used by beginners and then move to object-oriented programming (OOP), the C++ programming language. 

The reasoning behind the repository publication is to further my studies in the C++ programming language to include C++ templates along with C++ meta programming. Many in the industry would narrow the modern C++ language down by encapsulating it into a singularity called abstraction. Unfortunately, many like myself where the modern C++ abstraction is difficult to grasp.

## Libraries

- [Arduino Core](https://github.com/arduino/ArduinoCore-avr)
- [Arduino Libraries](https://www.arduino.cc/reference/en/libraries/)
- [PlatformIO Documents](https://docs.platformio.org/en/latest/)
- PlatformIO Project Configuration File [platformio.ini](https://docs.platformio.org/en/latest/projectconf/index.html)
- [PlatformIO Registry](https://registry.platformio.org/)
- MCUdude [MightyCore](https://github.com/MCUdude/MightyCore)

# References - Please note that all references will be removed in the near future...

## Quick Start

- Modern C++ in Embedded systems - [(YouTube)](https://www.youtube.com/watch?v=1l2g2dAobXA)
- Bare Metal C++ - [(Online Book)](https://alex-robenko.gitbook.io/bare_metal_cpp/)
- Compiler Explorer - [(Website)](https://godbolt.org/)
- An incomplete list of C++ compilers - [(Stroustrup C++ Website)](https://stroustrup.com/compilers.html)
- C++ Standards Support in GCC - [(Website with Technical Specifications Links)](https://gcc.gnu.org/projects/cxx-status.html)
  - This is the website to find the difference between the standards & the GCC versions.
- Free Books to Learn C++ [(Website with advertisements)](https://www.linuxlinks.com/excellent-free-books-learn-c-plus-plus/)

## Visual Studio Code - Quick Tutorial

- VS Code - Setup Makefile & Other Extensions [(YouTube 10 minutes)](https://www.youtube.com/watch?v=whQQF4kVjPY)

## Git and GitHub by using the VS-Code

- Introduction to Github and Git with Ubuntu [(YouTube 8 minutes)](https://www.youtube.com/watch?v=_kAV059yZ_s)
  - Although it's a short video pay attention to the terminal command 'git config'...
- Git and GitHub for Beginners - Crash Course by freeCodeCamp.org [(YouTube about 1 hour)](https://www.youtube.com/watch?v=RGOj5yH7evk)
  - Unlike the first video, it does not cover 'git config'..., but it covers a broad view.

## Lab Notebook: Science - Physics - Chemistry - Engineering - Electronics - Robotics

- Writing the Laboratory Notebook (US Department of Education) - [(PDF file)](https://files.eric.ed.gov/fulltext/ED344734.pdf)
     - I had printed this PDF file out into a binder to be used as a quick reference.
     - There are **not** many lab notebook **examples** to reference, so if anyone has a link, please pass it my way.
     - [ERIC - Institute of Education Sciences](https://ed.gov) 
- Laboratory Notebook with permanent numbered pages. Prices may range from 20 to 150 US dollars per notebook.
   - Scientific Notebook Company - [(Take a look at an example on lab notebooks)](https://snco.com)

## DIY Beginners Desktop Lab

- [Make a One Desk Electronics Lab](https://www.instructables.com/Make-a-One-Desk-Electronics-Lab-in-a-Small-Place-f/)
- [A DIY electronics lab for beginners](https://thesmarthomejourney.com/2020/10/12/diy-electronics-lab-desk/)
- Please Read the ***MageMCU Disclaimer***
- **Safety Data Sheets**, where to find **MSDS** and **SDS** on the internet... **Safety Comes First**.
	- OSHA Laboratory Safety Guidance [PDF](https://www.osha.gov/sites/default/files/publications/OSHA3404laboratory-safety-guidance.pdf)
	- OSHA Hazard Communication Safety Data Sheets [Quick Card PDF](https://www.osha.gov/sites/default/files/publications/OSHA3493QuickCardSafetyDataSheet.pdf)
	- Pb Lead-Free RoHS Exempt [PDF](https://web.calce.umd.edu/lead-free/SMTAExemptMay8.pdf)
- [Five essential tools for electronics lab safety](https://www.arrow.com/en/research-and-events/articles/five-essential-safety-products-for-every-electronics-lab)
- Parents and Teachers On Safety Transparency - I have been searching for a contractual agreement example for the school, teacher and parent when it comes to the student's safety [Safety Instructions PDF](https://cs.wmich.edu/gupta/teaching/cs5950/fall2011/safety%20instructions%20from%20International%20University%20Bremen.pdf). Although this is a very simple example, this agreement lacks a legal disclaimer. Furthermore, such an agreement can be made in a household with a DIY electornics labaratory between the parents and their children. As a warning, such laboratories may catch fire.
	- Recommended Agreement Information
		- Emergency Phone Numbers
		- Home Address
		- Contact Information
		- Legal Permissions for Hospitalization
		- Legal Disclaimer
		- Witness Name & Signature
		- Sign and Date
	- The motivation behind this type of an agreement, there is not enough all-around laboratories in our public schools for vocational readiness. Let's get America back to work.

## Recommended Beginners C++ Textbook

- Programming: Principles and Practice Using C++, 2nd Edition - [(Pearson - Learning. For life.)](https://www.pearson.com/us/higher-education/program/Stroustrup-Programming-Principles-and-Practice-Using-C-2nd-Edition/PGM270453.html)

	- [Author:](https://www.stroustrup.com/index.html) Bjarne Stroustrup's homepage.
	- [Source:](https://www.stroustrup.com/programming.html) More information on his book, PPP2.
	- [Support for PPP2](https://www.stroustrup.com/programming_support.html) This includes the source code for the book.
		- The source code has an excellent example in Chapter-24 on his ***matrix.h*** file.

## Recommended Electronics Textbook

- Introductory Circuit Analysis, 14th edition - [(Pearson - Learning. For life.)](https://www.pearson.com/store/p/introductory-circuit-analysis/P100001202025/9780133923605)
- Laboratory Manual for Introductory Circuit Analysis, 13th edition [Amazon](https://www.amazon.com)

## Tentative Disclaimer

- This page is meant for the author and belays with the author. If anyone disagrees with its content, please contact the author...

## Disclaimer and Terms

Please follow the ***Disclaimer*** and ***Terms*** in each of the Depositories here at MageMCU.

