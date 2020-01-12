## Basic Hardware Workshop ( Null Pune - 12-01-2020)

### Contents Discussed 

#### Introduction To Hardware

This section mainly  discussed about the basic hardware concepts that one needs to know before attacking any hardware.

 * Basic Concepts - Voltage, Common Ground Concept, Use of Level shifters, Concept of AC/DC
 * Components - Use of Resistor, Capacitor, transistor and possible attacks examples.
 * How to identify IC packages on Printed Circuit Boards.
 * Types of memory (SRAM, EEPROM, FLASH) mainly used in embedded devices and possible attcks exapmes related to it. 
 * Hardware tools that are generally used during attack. (Multimeter, UART_USB Adapter, Logic Analyzer, JTAG Scanners)

#### Hardware Attacks

 * Hardware Recon 
     * Ways to get internals of your hardware without actually buying the device (FCC ID - fccid.io)
     * Possible hardware attack surface 
     * Datasheets Importance and tricks
 * Attacking Debug Ports
     * Debug Port Introduction and Importance
     * JTAG Understanding
     * Hands on practical session :
        * To find JTAG Port on the hardware device (Hardware used in workshop - DIVA Board)
        * To dump the firmware using JTAG port, Expliot Nano, Openocd tool and Telnet , with commands mentioned in commands.md file.
        * To analyze the firmware using bless tool and fetch the secret key inside it.
        * Modify the password and patch the firware to the device.
        * Examples of the possible attacks that are possible if attacker founds the JTAG Port
 * Attacking Memory
      * Data storage
      * Memory chips and protocols
      * I2C Protocols
      * Hands on practical session :
        * To find I2C EEPROM chip on the hardware device (Hardware used in workshop - DIVA Board)
        * To dump the EEPROM data using Expliot Nano, Expliot Framework, with commands mentioned in commands.md file.
        * To fetch the data using bless tool (or strings command) and get the secret key inside it.
        * Modify the secret key and write to the I2C EEPROM of the device.
        * Examples of the possible attacks that are possible if attacker founds the  access to memory.

#### References :


 * https://www.elprocus.com/communication-protocols/
 * http://www.i2c-bus.org/repeated-start-condition/
 * http://www.i2c-bus.org/i2c-primer/how-i2c-hardware-works/
 * https://electricimp.com/docs/resources/spi/
 * https://learn.sparkfun.com/tutorials/serial-peripheral-interface-spi
 * https://blog.senr.io/blog/jtag-explained

 
