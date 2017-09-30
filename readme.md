# Raspberry-Pi-Zero-Rubber-Ducky-Duckberry-Pi

Version 1.0

A £10 Rubber Ducky USB HID!

## Introduction

DuckBerry Pi is a Raspberry Pi distro based on Minibian which allows the Raspberry Pi Zero to behave similar to a [USB Rubber Ducky](https://hakshop.com/products/usb-rubber-ducky-deluxe): a small device USB device which emulates a keyboard and automates key entry. Ducky scripts (uncompiled) which are made for the USB Rubber Ducky can be used with the Duckyberry Pi without modification. This can be useful for automating computer tasks, penetration testing machines, playing pranks, or just fun (by default plugging in an untouched Duckberry Pi image will open a Youtube video). Since it is recognized as a standard keyboard, this tool is compatible with Windows, Mac OS, Linux, Android, PlayStation 4, and anything that supports a USB keyboard.

## Getting Started

These instructions will help you setup and install your own Duckberry

### Instalation

1) Download the ISO for [Rasbian Lite 2016-02-29](http://downloads.raspberrypi.org/raspbian_lite/images/raspbian_lite-2016-02-29/)

2) Burn the ISO to the Micro SD Card - if you can't do this, [Google can help!](https://www.google.co.uk/search?q=burn+raspbian+lite+to+sd+card)

3) Version 1 includes a setup script that automates the setting up from version 0.5. Download this using wget.
    ``` bash
    wget https://raw.githubusercontent.com/ossiozac/Raspberry-Pi-Zero-Rubber-Ducky-Duckberry-Pi/master/duckysetup.sh
    ```

4) Make the script executable
    ``` bash
        chmod +x duckysetup.sh
    ```
   
5) Run the script
   ``` bash
       ./duckysetup.sh
   ```
   
### Using Duckberry
   
6) Turn off the PI, plug it into the target host machine via USB cable in the peripheral micro USB port, NOT THE POWER PORT.  A power cord is not required as the Pi Zero will take power directly from the host machine.
    
7) Watch the script execute on the host machine - You may have to plug it in twice, the first time installs drivers.

8) Once the video opens (defult script) take the SD card out of the PI, plug it into any machince with a USB SD card adaptor and then change /boot/payload.dd file to any DuckyScript Payload.

## Duckyscript

There are lots of [ready made ducky scripts here](https://github.com/hak5darren/USB-Rubber-Ducky/wiki/Payloads) and you can make your own with [this genorator](https://ducktoolkit.com/). Just make sure you use uncompiled Ducky Script .dd extension not .bin.

## Credits

Authors: Jeff L.
       : Dee-oh-double-gee
       : Theresalu
       : Ossiozac
       
Credits to Original Authors:
DroidDucky by Andrej Budincevic (https://github.com/anbud/DroidDucky)
hardpass by girst (https://github.com/girst/hardpass)

## MIT License

Copyright (c) [2017] [Zac Orehawa]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.