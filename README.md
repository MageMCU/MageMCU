# About MageMCU

<p align="center">
	<strong>--- Blinking LED ---</strong>
</p>

I'm Jesse. I've been fascinated by the magic of modern tech. My interest is in the AVR which is a family of microcontrollers developed by Atmel, acquired by Microchip but also expanding up from the 8-bitting devices.

I did put together a rudimentary robot to study the interfacing and programming of MCUs. The reasoning behind the repository publication is to further my studies in the C++ programming language to include C++ templates along with C++ meta programming. Many in the industry would narrow the modern C++ language down by encapsulating it into a singularity called abstraction. Unfortunately, many like myself where the modern C++ abstraction is difficult to grasp. Therefore, it would be nice to hear from others on improving the code. 

<p align="center">
	<img src="https://user-images.githubusercontent.com/87388066/192183593-076dc5a1-4fb2-4893-b88e-f223ffb8636a.jpg" width="400" />
</p>

The bare metal programming is done on the VS Code using the PlatformIO core but keep in mind the standard tools like GNU GCC C++11 or better. The electronic circuits may be displayed when appropriate. The MCU may be linked to other devices like another MCU in a master-slave relationship along with a bi-directional communication with an experimenting computing device. The communication types are presently I2C (SPI, IoT, RF Devices with emphasize RF Serial Communications Interface, Digital Modulation Shift-Keying). Finally, the type of robot used here is a simple two wheeled differential drive mobile agent.

# IC Components (Sensors) 

Embedded Programming levels use the Assembly, C amd C++ languages with the GNU C compiler (gcc) and assembler (as). 

Who is the sole responsible body for the hardware (IC Components) quality control and for the electronics software development? 

The manufacturer is responsible for the quality control of its own IC components including its software development using any one of the embedded programming language levels.

Assembler Language GNU C compiled firmware is compatible with the higher C languages which interacts directly with the IC hardware. The C language may be used instead or along with the assembly firmware of the IC component. The C++ language is used at an abstract level such as smart control systems using artificial intelligence. All programming levels work together where the manufacturer uses as a minimum standard to specify all levels of programming into their IC components in their datasheets (or Application Notes). No single enterprise should have a monopoly on any programming that might exclude the GNU C Compiler on their IC component.

Embedded systems interact directly with the real world like magnetometers to process sensor data and the results are used to interact with the real world by using actuators. The textbook by Stuart J. Russel and Peter Norvig called Artificial Intelligence, A Modern Approach, shows a figure of an intelligent agent interacting with the environment through sensors and actuators. Embedded programmers should place a large image of the figure above their computer especially the one with the BIG question mark.

Quality Control and Assurance is the responsibilty of everyone. The manufacture cannot be the sole individual responsible for SOME BAD APPLES. The IC components are mounted on boards if not by the manufacturer then by a third party PCB manufacturer. The client or customer should design a qualitative quantitative quality control test whether such boards are applicable under control methods on the sensor data. Does the board and IC component function as per the manufacture's contract...

I have a box called misty where I toss bad apples...

# References

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

- Introductory Circuit Analysis, 13th edition - [(Pearson - Learning. For life.)](https://www.pearson.com/store/p/introductory-circuit-analysis/P100001202025/9780133923605)
- Laboratory Manual for Introductory Circuit Analysis, 13th edition - [(Pearson - Learning. For life.)](https://www.pearson.com/store/p/introductory-circuit-analysis/P100001202025/9780133923780?tab=overview)

## Libraries

- Arduino - [(Library)](https://www.arduino.cc/reference/en/libraries/)
- PlatformIO - [(Registry)](https://registry.platformio.org/)

## Tentative Disclaimer

- This page is meant for the author and belays with the author. If anyone disagrees with its content, please contact the author...

## Disclaimer and Terms

Please follow the ***Disclaimer*** and ***Terms*** in each of the Depositories here at MageMCU.

