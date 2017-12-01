#How to use the Power Management Unit

You will find here how to install your PMU into your setup efficiently, as well as how to use current and voltage sensing.

###Soldering the battery cables

First of all, you'll need to solder your battery cables onto the PMU. You should solder your batteries on the _BATT IN_ solder pads, taking care of the polarity of your cable/battery and the one indicated on the top of the PMU case. You can use _XT60_ or _TPLUG_ connectors, and the module accepts up to 12S batteries.

[PIC Cables Soldered + Indications]

###
Next, you should plug one of your batteries to see the four LEDs of the module light up, and then plug the second one.

You'll then need to connect the power supply outputs to your autopilot. Using a Pixhawk 3 PRO autopilot, you'll simply have to use one of the 6 pins JST-GH cables shipped along the module to connect the (MAIN OUTPUT 1) from the PMU to your BRICK 1 port on the right side of the Pixhawk 3 PRO. The pinout of both connectors is ready to plug and doesn't need specific cables.

[PIC OUTPUT TO PIXHAWK]

If you're using another autopilot or device (ie. the Dropix autopilot [ADD LINK TO DRPOIX DOC WIRING]), you may want to take a look at the exact pinout of the PMU ([following this link](wire.md)) to see if the pinout is compatible with your device. You can adapt using customised cables. [ADD LINK?]

[PIC 1 BATTERIE]

If you're using two batteries, you can connect both (MAIN OUTPUTS) outputs from the PMU to your Pixhawk 3 PRO flight controller. This will provide redundant power supply to your main board and then improve the safety of your machine in case you're running low on one of your batteries. [CHECK DAMIEN SI DEPLETE EN MEME TEMPS]

[PIC 2 BATTERIES]

In the case you're using one battery, you can use both remaining JST-GH cables to connect the voltage sensing and current sensing signals to your autopilot's corresponding inputs. Again, the PMU is plug-and-play with the Pixhawk 3 PRO, for which you will find the corresponding connectors on the [COTE] of the board. For other autopilots, you might want to check the wiring of the PMU again ([following this link](wire.md)) before connecting it.

[PIC BOTTH SENSING]

If you're using two batteries, you'll need to use a fourth 6 pin JST-GH cable to connect both vooltage and current sensing signals. 