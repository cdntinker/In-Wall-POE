Designed to fit inside of Wiremold surface mount boxes.

Inspired by the EAP235-wall wireless access point which has pass-through PoE.  I have a little receiver for my weather station that connects to the network via WiFi & is powered by a USB charger.

Center hole, initially,  exists to make room for the Ethernet cable feeding the EAP235.  Of course, it can also allow for the cables to feed into the wall.

J1 supplies 5V output at up to 7W and can have a USB-A pigtail connected to feed devices outside the box.

The outline on layer User1 is the internals of a typical Wiremold surface box.

> [!NOTE]
> The outline on layer User2 in the board view is a fairly accurate representation of an Ethernet plug in position in the jack.
> 
> The outline on layer User3 is a fairly accurate representation of an Ethernet plug in the back of the EAP235.

> [!TIP]
> Actual board should fit in ANY North American box.

> [!TIP]
> The PoE module in use is available in 3v3, 5v0 and 12v versions.
> So, this board could also be used to supply those voltages.

> [!NOTE]
> See notations in the schematic and refer to the datasheet for information about resistors R1-R3.

2024/01/22: upgraded from the overkill Ethernet jack to a better fit plus magnetics...

2024/02/13: Assembled first board
* No smoke, but not producing output properly...
  * So far, suspect it needs more of a load.  Will test once I find a USB-A pigtail.
* Need to change footprint of L1 to something easier to hand-solder & move C1 a little to the left to make assembly easier.

2024/02/15: Tested successfully
* Definitely needs minimum load.
  * Added 2x 470 ohm resistors in parallel at R3 (Now Rl1 & Rl2)
* Does not seem to reliably keep voltage under much load.
  * Possibly because of knock-off module?  Must get Silvertel modules & test...
* Modified L1 footprint, moved C1 & added an extra load resistor footprint.  All to ease assembly.
