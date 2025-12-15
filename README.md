# Solid State Relay (SSR) using ESP32

## Overview

This project demonstrates the design and implementation of a Solid-State Relay (SSR) to control a high-voltage AC load (110V/220V) using a low-voltage 3.3V control signal from an ESP32 microcontroller. The system provides safe, silent, and reliable switching suitable for home automation and IoT applications.

## Key Features

* Contactless AC switching using a TRIAC-based SSR
* Galvanic isolation between low-voltage control and high-voltage AC mains
* Silent operation with no mechanical wear
* High reliability and long operational life

## Hardware Components

* ESP32 microcontroller
* BC547 NPN transistor (driver stage)
* MOC3033 optocoupler (non-zero-crossing)
* BTA41-600B TRIAC
* Resistors and indicator LED
* AC load (e.g., incandescent bulb)

## Working Principle

1. The ESP32 generates a digital control signal on a GPIO pin.
2. A BC547 transistor amplifies the GPIO signal to drive the optocoupler LED safely.
3. The MOC3033 optocoupler provides galvanic isolation and triggers the TRIAC.
4. The BTA41 TRIAC switches the AC load ON or OFF based on the control signal.
5. The TRIAC naturally turns OFF at the AC zero-crossing when the control signal is removed.


## Preview

[Watch Project Demo](https://youtube.com/shorts/_4SUz_vUINs?si=3yqj3TIjAa78iPeo)

## Applications

* Home automation systems
* IoT-based appliance control
* Industrial control interfaces
* High-voltage AC load switching

## Safety Note

This project involves high-voltage AC mains. Proper insulation, PCB clearances, and safety precautions must be followed during implementation and testing.

## Author

Ronak Bansal

