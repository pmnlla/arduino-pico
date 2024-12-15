# SEE UPSTREAM

Raspberry Pi Pico Arduino core, for all RP2040 and RP2350 boards

This is a port of Arduino to the RP2040 (Raspberry Pi Pico processor) and RP2350 (Raspberry Pi Pico 2 processor). It uses the bare Raspberry Pi Pico SDK and a custom GCC 14.2/Newlib 4.3 toolchain and supports ARM and RISC-V cores.


# Supported Boards
* VCC-GND YD-RP2040 (also represented as Generic)

# Installation
Follow internal guide published on GC.

# Uploading Sketches
To upload your first sketch, you will need to hold the BOOTSEL button down while plugging in the Pico to your computer.
Then hit the upload button and the sketch should be transferred and start to run.

After the first upload, this should not be necessary as the `arduino-pico` core has auto-reset support.
Select the appropriate serial port shown in the Arduino Tools->Port->Serial Port menu once (this setting will stick and does not need to be
touched for multiple uploads).   This selection allows the auto-reset tool to identify the proper device to reset.
Them hit the upload button and your sketch should upload and run.

In some cases the Pico will encounter a hard hang and its USB port will not respond to the auto-reset request.  Should this happen, just
follow the initial procedure of holding the BOOTSEL button down while plugging in the Pico to enter the ROM bootloader.

# Licensing and Credits
* The [Arduino IDE and ArduinoCore-API](https://arduino.cc) are developed and maintained by the Arduino team. The IDE is licensed under GPL.
* The [RP2040 GCC-based toolchain](https://github.com/earlephilhower/pico-quick-toolchain) is licensed under under the GPL.
* The [Pico-SDK](https://github.com/raspberrypi/pico-sdk) is by Raspberry Pi (Trading) Ltd and licensed under the BSD 3-Clause license.
* [Arduino-Pico](https://github.com/earlephilhower/arduino-pico) core files are licensed under the LGPL.
* [LittleFS](https://github.com/ARMmbed/littlefs) library written by ARM Limited and released under the [BSD 3-clause license](https://github.com/ARMmbed/littlefs/blob/master/LICENSE.md).
* [UF2CONV.PY](https://github.com/microsoft/uf2) is by Microsoft Corporation and licensed under the MIT license.
* Networking and filesystem code taken from the [ESP8266 Arduino Core](https://github.com/esp8266/Arduino) and licensed under the LGPL.
* DHCP server for AP host mode from the [Micropython Project](https://micropython.org), distributed under the MIT License.
* [FreeRTOS](https://freertos.org) is copyright Amazon.com, Inc. or its affiliates, and distributed under the MIT license.
* [lwIP](https://savannah.nongnu.org/projects/lwip/) is (c) the Swedish Institute of Computer Science and licenced under the BSD license.
* [BearSSL](https://bearssl.org) library written by Thomas Pornin, is distributed under the [MIT License](https://bearssl.org/#legal-details).
* [UZLib](https://github.com/pfalcon/uzlib) is copyright (c) 2003 Joergen Ibsen and distributed under the zlib license.
* [LEAmDNS](https://github.com/LaborEtArs/ESP8266mDNS) is copyright multiple authors and distributed under the MIT license.
* [http-parser](https://github.com/nodejs/http-parser) is copyright Joyent, Inc. and other Node contributors.
* WebServer code modified from the [ESP32 WebServer](https://github.com/espressif/arduino-esp32/tree/master/libraries/WebServer) and is copyright (c) 2015 Ivan Grokhotkov and others.
* [Xoshiro-cpp](https://github.com/Reputeless/Xoshiro-cpp) is copyright (c) 2020 Ryo Suzuki and distributed under the MIT license.
* [FatFS low-level filesystem](http://elm-chan.org/fsw/ff/) code is Copyright (C) 2024, ChaN, all rights reserved.
* [TLSF memory manager for PSRAM from Espressif fork](https://github.com/espressif/tlsf) of [original](https://github.com/mattconte/tlsf) by Matthew Conte is copyright Matthew Conte and licensed under the MIT license.
* [ESPHost library](https://github.com/Networking-for-Arduino/ESPHost) is LGPL licensed by its maintainers.

-Earle F. Philhower, III  
 earlephilhower@yahoo.com
