---
layout: default
title: Voltage step-down
parent: Hardware
nav_order: 3
permalink: /step_down
---

# Voltage step-down converter

The **Dagor Controller** has a DC-DC step-down (buck) converter (U3) that regulates the input voltage to 3.3V to power the microcontroller and the magnetic sensor and to be able to power external peripherals, such as: an external magnetic sensor, encoder, display, etc. This converter operates at a fixed 0.7mhz, implements soft-starting and has thermal shutdown.

![buck_converter_dagor](Images/buck_converter_dagor.png)

|         WARNING          |
|:---------------------------|
| Touching this IC may fatally damage the controller (the IC is label as U3 on the board).   |

It is possible to disconnect the output of the buck converter by removing the solder bridge shown in the picture bellow.

![solder_bridge](Images/solder_bridge.png)