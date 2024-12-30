# About MageMCU

<p align="center">
	<strong>--- Blinking LED ---</strong>
</p>

The *Hello World* cliche is still blinking... Hello, I'm Jesse. I've been fascinated by the magic of modern tech. My interest is programming the AVR which is a family of microcontrollers (MCU) developed by Atmel, acquired by Microchip.

## The two wheeled differential drive mobile robot

I did put together a rudimentary robot to study the interfacing and programming the MCU. Yet, there are many inexpensive two wheeled differential drive mobile robots (DDMR) on sale. Google the keywords ***Arduino Differential Drive Mobile Robot*** and then select the Google tab *Shopping*... The **MageMCU** repositories have experimental software that will work on these robots: two-wheels with caster, 4-wheels or tracks. The brains for the DDMR is the most used and popular **Arduino Uno Rev3** board (UNO). 

<p align="center">
	<img src="https://user-images.githubusercontent.com/87388066/192183593-076dc5a1-4fb2-4893-b88e-f223ffb8636a.jpg" width="400" />
</p>

## Atmega328P

At the heart of the **UNO** is the Atmega328P-PU (atmega328p) MCU. The 28-pin DIP package is easily replaced if damaged. Furthermore the **UNO** board with the atmega328p chip removed can be used as a programmer.
- The Arduino to a Microcontroller on a Breadboard [Uploading a Sketch Using an Arduino Board](https://docs.arduino.cc/built-in-examples/arduino-isp/ArduinoToBreadboard/)
	- Remove the atmega328p chip from the UNO in order to use the UNO as a programmer...
- See datasheet (pdf file) for the Atmega328P...

Note that **Bootloader** below clarifies and exemplifies the one described here...

## Atmega16U2 

The Atmega16U2 chip on the Arduino Uno board acts as a bridge between the computer's USB port and the MCU serial port. 
- [Updating the Atmega8U2 and 16U2 on an Uno or Mega2560 Using DFU](https://docs.arduino.cc/retired/hacking/software/DFUProgramming8U2/)
	- Note that updating this chip is rarely performed unless a new chip is placed on the UNO.
- See datasheet (pdf file) for the Atmega16U2...

## Bootloader

- [Burn the bootloader on UNO...](https://support.arduino.cc/hc/en-us/articles/4841602539164-Burn-the-bootloader-on-UNO-Mega-and-classic-Nano-using-another-Arduino#common-pins)
	- [UNO R3](https://docs.arduino.cc/hardware/uno-rev3/)
 		- [UNO R3 Schematic](https://docs.arduino.cc/resources/schematics/A000066-schematics.pdf)
			- Notice where in the schematic the TX-RX and the RX-TX connections cross between the atmega16u2 and the atmega328p. The wiring in a serial communication is connected such that the TX of one device like the atmega16u2 is connected to the RX of the other device like the atmega328p, and its RX is connected to the TX. Do not forget to connect the ground (GND) wire amoung all devices used...
- [Arduino as ISP for Arduino Bootloaders](https://docs.arduino.cc/built-in-examples/arduino-isp/ArduinoISP/)


## AVR Programming

- Many beginners use the [Arduino IDE software](https://www.arduino.cc/en/software).
- The advanced AVR programmers may use the [MS Visual Studio Code](https://code.visualstudio.com/) using the [PlatformIO core](https://platformio.org/). 
- [Bringing Arduino Into the Professional Environment](https://www.youtube.com/watch?v=EsEl9wDz_Y8)
- [AVR Professional Programming Software](https://www.microchip.com/en-us/tools-resources/develop/microchip-studio)
	- [Getting Started with Microchip Studio](https://www.youtube.com/playlist?list=PLtQdQmNK_0DQZjOQiqLyJwUcc88MJPOiD)
		- Note that the software ***Atmel Studio 7*** is now called ***Microchip Studio***.
- For the Raspberry Pi depending on the memory, the following editors will be used *Geany*, *Code::Blocks*, *MS VS Code* and *Arduino IDE*.

## Bare Metal Programming

- [Introduction to Bare Metal AVR Programming](https://www.youtube.com/watch?v=meGMw8K0NGk)
- [Practical Guide to Bare Metal C++](https://arobenko.github.io/bare_metal_cpp/)

## Make utility

- Study the AVR Tool Chain - Essential Guide used for Makefile - [Standard C library for AVR-GCC](https://www.nongnu.org/avr-libc/user-manual/overview.html)
	- [AVRdude Utility](https://github.com/avrdudes/avrdude)
		- This has a PDF file for AVRdude.
- [Using make and writing Makefiles](https://www.gnu.org/software/make/manual/make.html)
	- When writing a MakeFile that uses avr-gcc, avr-objcopy and avrdude, Google search the keywords: **Makefile mFile Atmega328P Github**. Learning how to use these **MakeFile** templates is a great way to understand the AVR Tool Chain.
   		- Use the following **make** [example](https://github.com/divayprakash/make/tree/master) as a guide while studying the AVR Tool Chain. Save a copy and expand those sections with additional comments (#) with a better description...

## Programming Language

- The procedural **C** prograomming language is used by beginners and then move to object-oriented programming (OOP), the **C++** programming language. 
- Programming: Principles and Practice Using C++, 2nd Edition - [(Pearson - Learning. For life.)](https://www.pearson.com/us/higher-education/program/Stroustrup--Programming-Principles-and-Practice-Using-C-2nd-Edition/PGM270453.html)
	- [Author:](https://www.stroustrup.com/index.html) Bjarne Stroustrup's homepage.
	- [Source:](https://www.stroustrup.com/programming.html) More information on his book, PPP2.
	- [Support for PPP2](https://www.stroustrup.com/programming_support.html) This includes the source code for the book.
- International Organization for Standardization (ISO) & Resources - [source](https://isocpp.org/std/the-standard)
	- ISO [Get Started](https://isocpp.org/get-started)
- C++ Reference - [source](https://en.cppreference.com/w/)
	- Standard Library [Headers](https://en.cppreference.com/w/cpp/standard_library)
 		- This is the reference for the Raspberry Pi...
 		- Archives for offline viewing - [source](https://en.cppreference.com/w/Cppreference:Archives) Use the *HTML ZIP file*
	- Be carefull when using the Standard (STD) Library with Arduino Boards.
 		- Use the [Arduino Documentation](https://docs.arduino.cc) instead of the STD Lib...
		- Arduino Docs - In the left column, select **Language Reference**
			- **Functions**
			- **Variables**
				- **Data Types** - Here you'll find **string** and **String()**
			- **Structure**
- *The reasoning behind the repository publication is to further my studies in the C++ programming language to include C++ templates along with C++ meta programming. Many in the industry would narrow the modern C++ language down by encapsulating it into a singularity called abstraction. Unfortunately, many like myself where the modern C++ abstraction is difficult to grasp.*

## Embedded Linux - Raspberry Pi
- GPIO in user-space
	- Raspberry Pi - [Whitepapers, App Notes & Compliance Guides](https://pip.raspberrypi.com/categories/685-whitepapers-app-notes-compliance-guides)
  		- [A history of GPIO usage on Raspberry Pi devices, and current best practices](https://pip.raspberrypi.com/categories/685-whitepapers-app-notes-compliance-guides/documents/RP-006553-WP/A-history-of-GPIO-usage-on-Raspberry-Pi-devices-and-current-best-practices.pdf) (pdf file)
   	- libgpiod library - GPIO character device
   		- Since linux 4.8 the GPIO **sysfs** interface is deprecated. User space should use the character device instead. This library encapsulates the ioctl calls and data structures behind a straightforward Application Binary Interface - ABI.
   	  	- [Bartosz Golaszewski - libgpiod](https://github.com/brgl/libgpiod) C library and tools for interacting with the linux GPIO
             character device (gpiod stands for GPIO device) A mirror of the original repository over at kernel.org. The github page is for discussions and issue reporting only. But, nice to see the code....
   		- [libgpiod library documentation](https://libgpiod.readthedocs.io/en/latest/index.html) this includes both C++ and Python bindings...
   		- [New GPIO Interface - Lloyd Rochester](https://lloydrochester.com/post/hardware/libgpiod-intro-rpi/)
   		- [New GPIO interface for linux user space](https://www.youtube.com/watch?v=BK6gOLVRKuU) Bartosz Golaszewski 2019
   		- [Linux GPIO: Evolution and Current State of the User API](https://www.youtube.com/watch?v=0APvuY2eLkY) Bartosz Golaszewski 2020
   	   	- [Libgpiod V2: New Major Release with a Ton of New Features](https://www.youtube.com/watch?v=6fxcDDLII6Y) Bartosz Golaszewski 2022
   		- [libgpiod GPIO-Manager](https://www.youtube.com/watch?v=tUFcWVwyzQg) Bartosz Golaszewski 2024
- I2C in user-space
	- Uses the ioctl call
- SPI in user-space
	- Uses the ioctl call

## Computers

- The Arduino integrated development environment (IDE) is a cross-platform application (for Microsoft Windows, macOS, and Linux operating systems)...
- Many older computers may be made to use a Linux operating system like Ubuntu which is recommended when connecting electronic circuits by USB because electrostatic discharge (ESD) may occur when the flow of electricity is interrupted along the circuit. For example, the data acquisition to your computer from a circuit running dc motors may well blow the USB circuit on the computer.
- The new Raspberry Pi 5 (Pi5) and its operating system is an inexpensive linux platform that is often used with the Arduino IDE. The Pi5 with 8GB has plenty of memory and processing power to run the Arduino IDE 2, VSCode with PlatformIO without any issues. If an ESD occurs on the Pi5 USB, the Pi5 can be replaced at a low cost...
	- This is what the author uses for AVR programming. 

## Libraries

- [Arduino Core](https://github.com/arduino/ArduinoCore-avr)
- [Arduino Libraries](https://www.arduino.cc/reference/en/libraries/)
	- [Arduino Reference](https://docs.arduino.cc/language-reference/) 
- [PlatformIO Documents](https://docs.platformio.org/en/latest/)
- PlatformIO Project Configuration File [platformio.ini](https://docs.platformio.org/en/latest/projectconf/index.html)
- [PlatformIO Registry](https://registry.platformio.org/)
- [RadioHead](https://github.com/epsilonrt/RadioHead) used for nRF24L01+ radio.
- [WiringPi](https://github.com/WiringPi/WiringPi) used to study its code but not recommended. See Embedded Linux above...

## Lab Notebook: Science - Physics - Chemistry - Engineering - Electronics - Robotics

- Writing the Laboratory Notebook (US Department of Education) - [(PDF file)](https://files.eric.ed.gov/fulltext/ED344734.pdf)
- Laboratory Notebook with permanent numbered pages.
  - Scientific Notebook Company - [(Take a look at an example on lab notebooks)](https://snco.com)

## Electronics Textbook

- Introductory Circuit Analysis author Robert L. Boylestad, 13th and now the new 14th edition
- Laboratory Manual for Introductory Circuit Analysis, 13th edition

## Electronics Courses

- Bad bad physics - from Maxwell's equations to Kirchhoff's Laws - don't fret it's all good - ha ha
	- [MIT OpenCourseWare - Circuits And Electronics](https://ocw.mit.edu/courses/6-002-circuits-and-electronics-spring-2007/) - Includes video lectures...
- Study **Ohm's Laws** while learning how to use the **Multimeter**
	- Say the following five times real fast...
 		- **amps ohms volts**
- [Oscilloscopes 101 for Engineering Students](https://www.youtube.com/playlist?list=PL2XuMA5AwNUznkBE46tcZAF3p5Edxgm-z)

## DIY Beginners Electronics Desktop Lab

- [Make a One Desk Electronics Lab](https://www.instructables.com/Make-a-One-Desk-Electronics-Lab-in-a-Small-Place-f/)
- [Electronics Lab Bench Setup Guide](https://www.reddit.com/r/electronics/comments/13ey0pb/electronics_lab_bench_setup_guide/?rdt=55016)
- [Making a Home Laboratory for Fun Projects](https://www.instructables.com/Making-a-Home-Electronic-Laboratory-Introduction-/)
- **Safety Data Sheets**, where to find **MSDS** and **SDS** on the internet... **Safety Comes First**.
	- [Lead - Safety Data Sheet (SDS)](https://beta-static.fishersci.com/content/dam/fishersci/en_US/documents/programs/education/regulatory-documents/sds/gsc-lead-safety-data-sheet.pdf) This is from Fisher Scientific.
	- [Lead Solder Alloy - Material Safety Data Sheet (MSDS)](https://hybridatelier.uta.edu/uploads/equipment/msds/4/24-6040-6401_msds.pdf) This is from University of Texas at Arlington.
	- [Tin/Lead Solid Solder - Safety Data Sheet (SDS)](https://weldcotemetals.com/SDS/Welding/sds-tin-lead-solid-solder.pdf) This is from Weldcote Metals.
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

## BUG FIXES

- In the Joystick.h file, the algorithm uses abs() function but it uses the (int) integer type instead of a float...
	- Has yet to be incorporated into the older repositories...
   	- I caught this while coding - Wireless Communication - nRF24L01
   	- As of 20240813, the code was added to MiscMath.h. See all header revisions in the include folder in both the *Wireless Communication* and the *Joystick Uno L298N* repositories.
```
   template <typename T>
    T absT(T val)
    {
        T zero = (T)0;
        if (val < zero)
            val *= (T)-1;
        return val;
    }
```
- The Joystick Uno L298N repository has been updated with this fix. Other issues including expanding the L298N Bits() function from eight (8) to sixteen (16) combinations which finishes with the Motor Movement Checklist (MMC). The article ***1009 - L298N Supplemental*** has been updated with more informtion in how to use the L298N Bits() function along with the MMC.

## Tentative Disclaimer

- Any products, services, and/or mediums like youtube videos described here on the ***MageMCU Github Account*** are considered unintentional and purely coincidental promotions and thereby to make clear any idea of such promotions should be interpreted solely as intended for the use for educational purposes only...
- **BUYER BEWARE** - this Github account uses links to Amazon marked as **Å** that reflects parts used. Transparency at this Github account is imperative.  All issues related to **Å** products should be directed to **Å**.
- The MageMCU Github account is actively hacking away on **experimental code** for the Arduino Uno Rev3. This includes testing and updating the software. Keep it simple.
- This page is meant for the author and belays with the author. If anyone disagrees with its content, please contact the author...
	- Jesse Carpenter doing business as Carpenter Software - Email: carpenter.software.jc@gmail.com
- Please follow the ***Disclaimers*** and ***Terms*** in each of the repositories including the Disclaimers and Terms by Github.
- MageMCU repository revised 20241230

