---
title: Powering Devices through the NMEA 2000 Network
weight: 1000
---

It is possible to power your custom devices via the NMEA 2000 network. To stay compliant with the NMEA 2000 specification and to ensure safe and uninterrupted operation of the NMEA 2000 network, it is important to observe some restrictions in the device connections.

[Galvanic isolation](https://en.wikipedia.org/wiki/Galvanic_isolation), or just isolation in short, is at a central role here.
Isolation is a technique to prevent the flow of electric current between two circuits.
At heart, it means that the two circuits do not share electrical ground.
This can be tested by measuring contiuity between the two circuit ground wires.
If there is no continuity, the circuits are isolated from each other.

The following diagrams illustrate the valid powering schemes.
In the diagrams, dashed lines illustrate the isolation barrier. 
Note that even though the figures and captions refer to the SH-RPi, the same rules apply to all other devices such as the SH-ESP32.

{{< imgrel "Power-diagram-n2k-and-power.png" "50%" >}}
Always OK: SH-RPi powered with a dedicated power cable.
{{< /imgrel >}}

{{< imgrel "Power-diagram-pure-n2k.png" "50%" >}}
OK: SH-RPi powered via the NMEA 2000 network, no external connections.
{{< /imgrel >}}

{{< imgrel "Power-diagram-unisolated-conx.png" "50%" >}}
OK: SH-RPi powered with a dedicated power cable and connected to external devices with a galvanic connection such as USB or unisolated RS-422.
{{< /imgrel >}}

{{< imgrel "Power-diagram-isolated-conx.png" "50%" >}}
OK: SH-RPi powered via the NMEA 2000 network and connected to external devices with an isolated connection such as Ethernet or isolated NMEA 0183.
{{< /imgrel >}}

{{< imgrel "Power-diagram-isolated-peripherals.png" "50%" >}}
OK: SH-RPi powered via the NMEA 2000 network having peripherals such as keyboard, mouse, or a GPS receiver that are powered by the Raspberry Pi and not connected elsewhere.
{{< /imgrel >}}


{{< imgrel "Power-diagram-illegal.png" "50%" >}}
Not permitted: SH-RPi powered via the NMEA 2000 and connected to external devices with a galvanic connection. This setup will cause a lot of noise and may impact the reliability of the Raspberry Pi or other devices.
{{< /imgrel >}}

