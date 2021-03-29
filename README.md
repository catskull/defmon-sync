# defMon Sync Adapter 
This is an adapter for the Commodore 64 computer. It is used to synchronize a tracker called [defMon](https://www.vandervecken.com/defmon/doku.php?id=download:download) with other music equipment.

It connects to the user port and outputs the following signals:
- LSDJ sync signal.
- nanoloop sync signal.
- midi clock.
- din sync.
- clock signal with adjustable resolution from 24ppqn to 2ppqn for Korg Volcas, TE Pocket Operators, Arturia Microbrute, MI Anushri etc.

It can only work as master.

It should also work with Prophet64.

# Purpose
ScannerBoy originally created and sold these devices but has since stopped. Due to demand, this is an effort to make hardware. To aid in this, the code is being ported to Arduino/MiniCore.

## Building/Flashing
- Install Arduino IDE (1.8.13)
- [Install MiniCore](https://github.com/MCUdude/MiniCore)
- Download/clone this repo and open the defmon-sync.ino file
- Select ATmega8 board from the boards dropdown
- For clock, selecte "External 20 MHz"
- Leave other options the defaults
- Connect a USB-serial adapter to the onboard FTDI header
- Select the serial port in Arduino menu, and hit upload!

# Credits
Original developer: Krzysztof Iwanowski

Additional PCB work by Orgia Mode

Arduino port by catskull

# License
The firmware, PCB layouts and schematics are released under a Creative Commons cc-by-sa 3.0 license.