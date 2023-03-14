---
title: NMEA 2000
weight: 1000
no_list: false
---

## Introduction

NMEA 2000 is a networking standard for marine electronics, used by most modern marine electronics hardware.
It is is constructed from a a number of devices connected to a single bus, called the network backbone.
All devices on the network can both transmit and receive messages.

An illustration of a typical NMEA 2000 network with some example devices is shown below.

{{< imgrel "nmea2000-diagram.svg" "70%" >}}
Example NMEA 2000 Network.
{{< /imgrel >}}

Figure components are:

<dl>
<dt>1</dt>
<dd>N2K power cable. Every NMEA 2000 network segment must be connected to boat's 12 V power system. Ideally, the power connection should be roughly in the middle of the backbone.</dd>
<dt>2</dt>
<dd>Network male and female terminators.
   The network backbone must be terminated with 120 ohm resistors for proper network operation. The are mandatory and essential!</dd>
<dt>3</dt>
<dd>Drop cables are connected to the backbone using T-connectors.
   The T-connectiors can have one or multiple drop cable connections.</dd>
<dt>4</dt>
<dd>Backbone cables extend the backbone. The maximum length of the network, measured from terminator to terminator,
   should not exceed 100 m.</dd>
<dt>5</dt>
<dd>Drop cables connect individual devices to the backbone.
   The maximum length of the drop cable is 6 m.</dd>
<dt>A</dt>
<dd>A display device such as a Multi-function Display (MFD).</dd>
<dt>B</dt>
<dd>A wind sensor.</dd>
<dt>C</dt>
<dd>A temperature sensor.</dd>
<dt>D</dt>
<dd>An SH-wg device.</dd>
</dl>

The network backbone is shown in pale blue color.
All devices connect to the backbone using drop cables.
Only one device can be connected to a single drop cable.

At the very minimum, the network must have a 5-way T-connector, two terminators, a power connection, and two devices with their own drop cables.

