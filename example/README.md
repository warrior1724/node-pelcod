﻿# Example of node-pelcod

This example show how to comunicate with a pelco d camera and control it from a webpage

[Youtube video](https://www.youtube.com/watch?v=MRMotnNFLpw)

## Getting Started

First you need to connect your Pelco D camera to a USB RS485 adapter (or to a USB RS232 adapter which has a RS232 to RS485 converter fitted).   [RS485 uses 2 wires for the transmit data, RS232 uses 1 wire].

Then install the software
```
$ git clone https://github.com/Scoup/node-pelcod
$ cd node-pelcod/example
$ npm install
$ bower install
$ echo Remember to change server.js and script.js with serial port and IP address settings (see below)
$ node server.js
```
*Obs: install [bower](https://github.com/bower/bower) if don't have it

Next change the path of serial port in server.js here: `new SerialPort("/dev/ttyUSB0"...`, the "/dev/ttyUSB0" to your own path. On Windows the path is "COM1".

The default Pelco D address camera is 0x01.

Open your browser in http://your_ip:8000 and then using a swipe you can Pan and Tilt the camera.

## License

The MIT License (MIT)

Copyright (c) 2014 Léo Haddad M. C. Carneiro

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.