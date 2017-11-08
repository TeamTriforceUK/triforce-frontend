# triforce-frontend

## Introduction

### Repository Navigation
This repository is one of two repositories hosting the codebase for the Triforce robot. The repositories are versioned and released seperately. Links to the repositories are below.

#### [Triforce Control](https://github.com/TeamTriforceUK/triforce-control)

The Triforce Control firmware (mbed OS) runs on an LPC1768 (ARM Cortex M3). The firmware is responsible for controlling the robot.

#### [Triforce Telemetry](https://github.com/TeamTriforceUK/triforce-telemetry)

The Triforce Telemetry repository hosts firmware (FreeRTOS) for the ESP8266 WiFi chip. This microcontroller works alongside the mbed to provide telemetry functionality via an HTTP server.

The ESP8266 allows us to communicate telemetry from Triforce to connected mobile devices (tablets, laptops, mobile phones). We also control non-safety critical settings such as LED lights from the mobile device.

#### [Triforce Frontend](https://github.com/TeamTriforceUK/triforce-frontend)

Web frontend provided by triforce-telemetry server. The frontend is provided as a git submodule to triforce-telemetry.

## System Overview

### Microprocessors

| Device  | Firmware  | Language |
|---------|-----------|----------|
| [LPC1768](https://developer.mbed.org/platforms/mbed-LPC1768/) | [mbed OS](https://www.mbed.com/en/development/mbed-os/)   | C++      |
| [ESP8266](https://www.adafruit.com/product/2471) | [FreeRTOS](http://www.freertos.org/)  | C        |

### Sensors

| Sensor | Purpose                              | Communication |
|--------|--------------------------------------|---------------|
| [BNO055](https://learn.adafruit.com/adafruit-bno055-absolute-orientation-sensor/overview) | Orientation, direction, acceleration |  I2C          |

## Development Environment

Any text editor and any popular web browser should do the job for basic frontend development.
Any more sophisticated changes should be tested on `triforce-telemetry`.

## Contributing

We are open to any contributions in terms of ideas, suggestions, bug reports, development. Feel free to open GitHub issues regarding any contributions.

## Licensing

This software is licensed under the [MIT License](https://tldrlegal.com/license/mit-license), unless stated otherwise.
