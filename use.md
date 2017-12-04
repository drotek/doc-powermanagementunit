#How to use the Power Management Unit

You will find here how to install your PMU into your setup efficiently, as well as how to use current and voltage sensing.

_ **Note: All along the setup of the PMU, be careful of never touching the inner boards of the module when the batteries are connected to the PMU to avoid any electrical shocks! ** _

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

_Note: For safety reasons, take care of closing the case and setting up the top case part again in order to prevent any electrical shocks._

You'll then need to connect the power supply outputs to your autopilot. Using a Pixhawk 3 PRO autopilot, you'll simply have to use the 6 pins JST-GH cables shipped along the module to connect the **POWER1** from the PMU to your **POWER1** port on the left side of the Pixhawk 3 PRO, and the **POWER2** output from the PMU to the corresponding **POWER2** input of the autopilot. The pinout of both connectors is ready to plug and doesn't need specific cables.

<p align="center">
  <img src="./images/con1.jpg?raw=true" alt="PMU connected pix"/>
</p>

Even in case you use a single battery and use both **POWER** outputs to power your Pixhawk 3 PRO autopilot to use its power redundancy ability, if the **POWER1** output is disfunctioning, the second output **POWER2** can supply power to your autopilot and keep it working, _whether you're using one or two batteries_.

If you're using another autopilot or device (ie. the Dropix autopilot), you may want to take a look at the exact pinout of the PMU ([following this link](wire.md)) to see if the pinout is compatible with your device. You can adapt using customised cables. 

<p align="center">
  <img src="./images/con2.jpg?raw=true" alt="PMU connected pix"/>
</p>

After connecting the PMU to your autopilot, you can connect a battery to the PMU to check the correct functionning of your system, seeing your autopilot turn up and boot normally. After that, you will need to install the PMU onto you machine, be it a drone, rover, or any other device!

###Powering your ESCs

The PMU can also provide a power supply bay, outputting the battery input directly out of the PMU to make soldering your ESCs directly onto the PMU possible.

To do so, you'll need to solder your ECSs' power cables onto the **BATT OUT +** and **BATT OUT -** soldering pads of the PMU. 

[PIC ESCs soldered]