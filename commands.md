## Commands

* Debug Port Attack (commands for Host machine)
    * `ls /dev/tty*` (Identify port for arduino and DIVA)
    * `sudo screen /dev/ttyUSB0 115200` (for arduino check; use ls /dev/tty* to verify port)
    * `sudo screen /dev/ttyACM0` (for DIVA Access)
    * `openocd -f /path/to/expliot_nano_jtag.cfg`
    * `telnet localhost 4444`
    * `reset halt` (command for openocd via telnet)
    * `dump_image /path/to/firmware1.bin 0x8000000 0x7FFFF`(command for openocd via telnet)
    * `bless firmware1.bin` (command on Host machine)
    * `flash write_image erase /path/to/firmware2.bin 0x8000000` (command for openocd via telnet)
  
* Memory Attack 
    * `sudo expliot` (command for Host machine)
    * `run i2c.generic.readeeprom -c 24AA256 -w filename.bin` (command for expliot framework)
    * `bless filename.bin` (command for Host machine)
    * `run i2c.generic.writeeeprom -c 24AA256 -r "fileModifiedName.bin"` (command for expliot framework)
  

