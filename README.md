## About MageMCU - Under Construction - ETC - Who knows!?

<p>
Hello World! My name is Jesse. I've been fascinated by the magic of modern tech. There was a time when I was living in a world when slide rules with its 3 significant digits were the norm. Today, there are millions and millions of hidden miniature computers everywhere even on our own person. The magic or the so-called wise-device, the MageMCU, (a name by the way chosen for this topic) is not a person but a computing device. The acronym MCU is a Micro Controller Unit. My interest is in the AVR which is a family of microcontrollers developed by Atmel, acquired by Microchip. These devices find many applications as embedded systems. One might imagine the feeling of what the word embedded might invoke and most likely would be correct in their assumption. They are modernly common in hobbyist and educational embedded applications, popularized by their inclusion in many of the Arduino line of open hardware development boards. By the turn of the century, Atmel had shipped 500 million AVR flash microcontrollers.
</p>

<p>
I am presently cleaning out (updating) the file cabinet full of old articles on algorithms for a variety of subjects in robotics, a part-time hobby. Although I am not an engineer, I did put together a rudimentary robot to study the interfacing and programming of MCUs. The reasoning behind the repository publication is not to show off my ignorance but to further my studies in the C++ programming language to include C++ templates along with C++ meta programming. Many in the industry would narrow the modern C++ language down by encapsulating it into a singularity called abstraction. Unfortunately, many like myself where the modern C++ abstraction is difficult to grasp. Therefore, it would be nice to hear from others on improving the code. This way when updating the articles I won't be wondering if whether I've mis-written another bug.
</p>

<p>
Please keep in mind that the memory size is quite small for the embedded firmware. The MCU used is the ATmega328P on a protoboard (breadboard). Actually any MCU will do but as many bitbangers may well know, this particular 8-bit device is quite popular. The AVR architecture has two main memory spaces, the Program Memory space (32 kilobytes flash memory), the Data Memory space (2 kilobytes internal SRAM) and besides the main memory spaces, there is another, the EEPROM Memory for data storage (1 kilobytes). Atmel's datasheet on this chip had 450 pages but today, Microchip narrowed it down to 294.
</p>

<p>
The bare metal programming is done on the VS Code using the PlatformIO core but keep in mind the standard tools like GNU GCC C++17 or better. The electronic circuits may be displayed when appropriate. The MCU may be linked to other devices like another MCU in a master-slave relationship along with a bi-directional communication with an experimenting computing device. The communication types are presently I2C (and maybe later SPI). Finally, the type of robot used here is a simple two wheeled differential drive mobile agent. Finally, I use for testing embedded systems with a linux computer with an old computer. The iMac which is old and neglected where it uses an up-to-date OS, the Debian Unbuntu 20.04 version and It Works!
</p>

### References
- [Modern C++ in Embedded systems - YouTube](https://www.youtube.com/watch?v=1l2g2dAobXA)
- [Bare Metal C++ - Online Book](https://alex-robenko.gitbook.io/bare_metal_cpp/)
- [Compiler Explorer - Unbelievable Website](https://godbolt.org/)
- [C++ Standards Support in GCC - Must Know](https://gcc.gnu.org/projects/cxx-status.html)
- [PlatformIO](https://platformio.org/)
- [Ubuntu OS](https://ubuntu.com/)
