# Esp32_ST7789_Pacman
 Remake of the famous pac-man, with some improvements

<img src="https://github.com/pdropes/Esp32---Pac-man/blob/main/doc/pac-man%20top.jpg" width=1024>

!!! NOTICE !!!


## Prepare
- This board was designed to be possible to do at home; the battery is the BL-5B or BL-5C, and the speaker is 32ohms from the 3310.
- In difficulty to find all components, the layout must be changed to support different ones.


## Development Environment
- [Arduino IDE](https://www.arduino.cc/en/main/software)
- [arduino-esp32](https://github.com/espressif/arduino-esp32)

1º Connect the board via USB to the PC.

2º The top buttons are for programming, on the left, IO0, on the right, RESET micro.
For the microcontroller to enter programming mode, the IO0 button must be held down while pressing the reset button briefly.

3º In the Arduino environment, choose "ESP32S2 Dev Module" board.

4º Upload, done.


## Controller
All commands are made on board by switches
LEFT-RIGHT-UP-DOWN , BUTTON A for new game, BUTTON B for pause


## Coding reference
- [Pacman-Arduino-Due](https://github.com/DrNCXCortex/Pacman-Arduino-Due)
- [esp32_ILI9328_Pacman](https://github.com/MhageGH/esp32_ILI9328_Pacman)


Changes:

- Schematic and connections for prototype
- ST7789 support
- Sounds trought two ESP32 8b DAC channels (ambient / effects)
- Functions of buttons A and B
- Show frightened ghosts blinking, before changing to normal
- Battery capacity monitor
- Hiscore saved in internal flash
- Slide-switch to select mode "off/charge" "on/mute" "on/sound"

It was my first time programming in C, it may not be perfect.
