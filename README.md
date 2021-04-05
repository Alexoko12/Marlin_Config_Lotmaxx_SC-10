# Marlin_Config
In this repo are sample config files for the use of Marlin with a Lotmaxx SC-10 running on an MKS Robin Nano v1.1 board.
# How To
1. Clone correct Marlin release from https://github.com/MarlinFirmware/Marlin/releases
2. Copy from here the files from Marlin-\<release\> to cloned marlin.
3. Modify configs and version as you need.
    * If you only want to add BL_Touch and keep everything default just uncomment "//#define LOTMAXX_BLTOUCH" and make sure you connected the probe as shown in the wiring diagram.
4. Compile with platformio.
5. Copy .pio/build/mks_robin_nano35_lotmaxx/Lotmaxx.bin to sd root.
6. Insert SD and start printer. It will flash automaticly and rename Lotmaxx.bin to LOTMAXX.CUR (If you want to flash again, just rename it back to Lotmaxx.bin).
7. Reset EEPROM.
8. Optional. If you have display problems after flashing put the Lotmaxx_font and Lotmaxx_pic folder to the root of the sd card with the Lotmaxx.bin and reflash the firmware again.
# Credit
Thank you to Daniel A Robertson for sharing his wiring diagram for autoleveling with BL_Touch.
# Disclaimer
I am not responsible for any failures by running this code. Please validate the config files before compiling marlin for your printer. And keep always an eye on your printer.
