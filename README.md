# OGK-SiPM-Board
🖸 OpenGammaKit PCB module designed for the 6 mm C-Series MicroFC-60035 SiPM in KiCad

## Description

This carrier board is designed for the 6 mm C-Series MICROFC-60035-SMT silicon photomultiplier (SiPM) by [onsemi](https://www.onsemi.com/pdf/datasheet/microc-series-d.pdf). It was developed specifically for the [OpenGammaKit](https://github.com/vikulin/OpenGammaKit/) detector, but it can also be used in other systems. An optional circuitry for automatic SiPM temperature gain compensation is included.

On the **front side**, only the sensor is mounted, while all supporting components are placed on the **back side**. This layout provides optimal optical coupling and ensures light-tight sealing. The unused SiPM pin 4 is tied to the ground pad, adding thermal mass and connecting it to the ground plane, where the NTC is also located.

The PCB integrates the recommended SiPM biasing filter and optional temperature compensation. To enable them, solder all required components and connect wires to the **PS** and **GND** pads. The SiPM signal output is available at the **anode (A)** pad.

The temperature compensation design is based on the paper *[“Temperature-Compensated Silicon Photomultiplier”](https://doi.org/10.1016/j.nima.2017.11.060)* by Evgeny Kuznetsov. Most of the research and testing for this board was carried out by **@sebyon** — many thanks for the contribution!
