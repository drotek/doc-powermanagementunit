#How to use the Power Management Unit

You will find here how to install your PMU into your setup efficiently, as well as how to use current and voltage sensing.

###Soldering the battery cables

Before soldering the battery cables onto your PMU, you will need to open the top part of the PMU in order to access the soldering pads easily. To do so, use a 2.5 mm Torx screwdriver to unscrew the top of the case open.

<p align="center">
  <img src="./images/use1.jpg?raw=true" alt="Unscrewed PMU Case"/>
</p>

<p align="center">
  <img src="./images/use2.jpg?raw=true" alt="Open PMU Case"/>
</p>

After opening the case, you'll need to solder your battery cables onto the PMU. You should solder your battery cables on the _BATT IN_ solder pads, taking care of the polarity of your cable/battery and the one indicated on the top of the PMU case along with details below. You can use _XT60_ or _TPLUG_ connectors, and the module accepts up to two simultaneously plugged 12S batteries.

<p align="center">
  <img src="./images/pads.png?raw=true" alt="PMU Pads description"/>
</p>

<p align="center">
  <img src="./images/sold.png?raw=true" alt="PMU cables soldered"/>
</p>

Next, you should plug one of your batteries to see the four LEDs of the module light up, and then plug the second one.

<p align="center">
  <img src="./images/leds.jpg?raw=true" alt="PMU Light up"/>
</p>

###Power distribution

You'll then need to connect the power supply outputs to your autopilot. Using a Pixhawk 3 PRO autopilot, you'll simply have to use one of the 6 pins JST-GH cables shipped along the module to connect the **POWER1** from the PMU to your **POWER1** port on the left side of the Pixhawk 3 PRO. The pinout of both connectors is ready to plug and doesn't need specific cables.

<p align="center">
  <img src="./images/con1.jpg?raw=true" alt="PMU connected pix"/>
</p>

If you're using another autopilot or device (ie. the Dropix autopilot), you may want to take a look at the exact pinout of the PMU ([following this link](wire.md)) to see if the pinout is compatible with your device. You can adapt using customised cables. 

If you're using two batteries, you can connect both **POWER1** and **POWER2** outputs from the PMU to your Pixhawk 3 PRO flight controller on the corresponding inputs. This will provide redundant power supply to your main board and then improve the safety and flight time.

<p align="center">
  <img src="./images/con2.jpg?raw=true" alt="PMU connected pix"/>
</p>
