---
title: NMEA 2000 Power Feed
weight: 1000
---

This page describes how to power the NMEA 2000 network.

## Connecting the Network Power Feed, Theory

The NMEA 2000 network supplies power to devices connected to it.
Even though some devices are externally powered, power connection is a mandatory part of the network. No data can be transmitted without it.

The voltage of the network is 12 V DC. If your boat has a 24V nominal electrical system, you must use a 24V to 12V DC converter to power the network.

The maximum current draw of the network is 3 A.
The network must be fused with a 3 A fuse to protect the network wiring.

The NMEA 2000 network should always be connected using a switch. Without a switch, the network is always powered on and the devices will deplete the boat battery.

Finally, the NMEA 2000 shield, or the braided sheath coveering the inner cable pairs, must be connected to the boat's ground at the power connection point. This is important for proper network operation because it prevents electrical noise from alternators, starter motors, inverters and other high current devices from interfering with the network.

A schematic of the network power connection is shown below.


{{< imgrel "nmea2000-power-connection.svg" "75%" >}}
NMEA 2000 Power Connection
{{< /imgrel >}}


## Connecting the Network Power Feed, Practice

Step by step instructions for connecting the network power feed are shown below.

First, cut the power cable to length. The cable should be long enough to reach the power connection point from the network backbone T-connector. Leave some slack, though -- nothing is more annoying than a cable that is too short!

{{< imgrel "wire1.jpeg" "75%" >}}
Cutting the cable to length
{{< /imgrel >}}


Strip the outer sheath of the NMEA 2000 power cable.
Required length depends on the location of the power connection point.
If the 12V and ground connections are close to each other, the cable can be cut to as short as 5 cm (2 in), but if the 12V and GND connection poits are separated, make the wires accordingly longer.

You can use sharp knife or a dedicated wire stripper, but be careful not to cut the shield braiding. You can use the off-cut from the previous step to practice and perfect your skills.

{{< imgrel "wire2.jpeg" "75%" >}}
Outer sheath stripped
{{< /imgrel >}}


Undo the shield braiding and cut it away. You'll find a twisted bare shield wire as well. Do not cut it, it'll be used later.

{{< imgrel "wire3.jpeg" "75%" >}}
Outer sheath stripped
{{< /imgrel >}}


Strip the foil shield from the wires.

Cut the blue and white signal wires away. The signal wires are not used in the power connection. Leave short stubs of the signal wires to prevent them from shorting to the shield strands.

{{< imgrel "wire4.jpeg" "75%" >}}
Wires ready
{{< /imgrel >}}


Slide a bit of larger diameter heat shrink tube on top of the whole cable. Then, cover the signal wire stubs with a bit of smaller diameter heat shrink tube. Also cover the bare shield wire with a bit of heat shrink tube. In the photo below, the signal wires are covered with yellow tube and the shield wire is covered with transparent tubing.

{{< imgrel "wire5.jpeg" "75%" >}}
Heat shrink tubes in place
{{< /imgrel >}}


Apply heat to shrink the heat shrink tubes, first to the smaller diameter ones, then to the larger one. In the photo below, the larger diameter heat shrink tube has some hot glue coating. That results in a thicker but more or less waterproof protection.

Strip the red and black wire insulation. The length depends on the type of terminals, but about 6 mm (1/4 in) is usually adequate.

{{< imgrel "wire6.jpeg" "75%" >}}
Wires stripped
{{< /imgrel >}}


Crimp suitable terminals to the wires: one terminal to the red wire and one for both the black wire and the shield.

Depending on your electrical panel, you can use wire end ferrules or small ring or spade terminals, as shown in the photo below.

{{< imgrel "wire7.jpeg" "75%" >}}
Terminal connectors
{{< /imgrel >}}


Connect the black wire and the shield to the ground terminal in the electrical panel. Connect the red wire to the 12V terminal. The 12 V circuit must be fused with a 3 A fuse or a circuit breaker. 

If you don't have an electrical panel on your boat, you can install an inline fuse holder and a separate switch to the red wire. In that case, you can use butt connectors or solder the wires together.

Finally, connect the network connector to a T-connector on the network backbone, and you are done!