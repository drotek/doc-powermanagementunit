# How to use

You will find here how to install your PMU into your setup efficiently, as well as how to use current and voltage sensing.

> _**All along the setup of the PMU, be careful of never touching the inner boards of the module when the batteries are connected to the PMU to avoid any electrical shocks!**_

## Soldering the battery cables

Before soldering the battery cables onto your PMU, you will need to open the top part of the PMU in order to access the soldering pads easily. To do so, use a 2.5 mm Torx screwdriver to unscrew the top of the case open.

![](.gitbook/assets/use1.jpg)

After opening the case, you'll need to solder your battery cable onto the PMU. You should solder your battery cable on the _BATT IN_ solder pads, taking care of the polarity of your cable/battery and the one indicated on the top of the PMU case along with details below. You can use _XT60_ or _TPLUG_ connectors, and the module accepts up to two simultaneously plugged 12S batteries.

![](.gitbook/assets/use2.jpg)

### Using a single battery:

If you plan on using a single battery, it won't be necessary to solder two battery connectors to the PMU. You should simply solder your cable onto the corresponding soldering pad on the right, taking care of the polarity. You can help yourself with the picture below.

## Powering your ESCs

The PMU can provide a power supply bay, outputting the battery power directly out of the PMU to make soldering your ESCs directly onto the PMU possible. To do so, you'll need to solder your ESCs' power cables onto the **BATT OUT +** and **BATT OUT -** soldering pads of the PMU, taking care of the polarities of your ESC's cables. You may want to keep the case opened in order to do this soldering operation.

![](.gitbook/assets/esc.jpg)

## Power distribution

> _For safety reasons, take care of closing the case and setting up the top case part again in order to prevent any electrical shocks._

Whether you use one or two batteries, the PMU will provide two independent power sources. This way, if you're using an autopilot that's _redundant-power-supply ready_, you'll be able to have your autopilot supplied power in a safer way, the second BEC replacing the first one if it happens to fail.

Using a Pixhawk 3 PRO autopilot, you'll simply have to use the 6 pins JST-GH cables shipped along the module to connect the **POWER1** from the PMU to your **POWER1** port on the left side of the Pixhawk 3 PRO, and the **POWER2** output from the PMU to the corresponding **POWER2** input of the autopilot.

If you're using another autopilot or device \(ie. the Dropix autopilot\), you may want to take a look at the exact pinout of the PMU \([following this link](hardware/wire.md)\) to see if the pinout is compatible with your device. You can adapt using customized cables.

![](.gitbook/assets/con2.jpg)

After connecting the PMU to your autopilot, you can connect a battery to the PMU to ensure the proper functioning of your system, seeing your autopilot turn up and boot normally. After that, you will need to install the PMU onto you machine, be it a drone, rover, or any other device!

