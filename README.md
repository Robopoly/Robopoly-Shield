# Robopoly shield

![Robopoly sheild](https://raw.github.com/Robopoly/Robopoly-Shield/master/shield.png)

This Arduino compatible shield is intended to work with the [EPFL Robotics club](http://robopoly.epfl.ch/) robotics platform [PRismino](https://github.com/Robopoly/PRismino). It can run on any Arduino as the pin placement is the same. The [PRismino library](https://github.com/Robopoly/prismino-library) makes it easy to use with shortcut definitions and functions.

## Characteristics

The shield has various input and output components to expand the PRismino's capabilities:

* Button
* 4 channel DIP-switch
* 2 standard servo motor connections
* Buzzer
* 2 channel H-bridge ([DRV8833](http://www.ti.com/product/drv8833)) with connectors
* Potentiometer
* I2C output with a micromatch connector
* Footprint for a HC-05 Bluetooth module
* 3-pin connector for power from the [Robopoly power board](https://github.com/Robopoly/Power-Board)

**NOTICE**: certain components that source current are wired to the MCU pins and **may damage it if those pins are configured as outputs**, please read carefully the [PRsimino library documentation](https://github.com/Robopoly/prismino-library) to avoid it.

Some elements like the button, buzzer and potentiometer can be disabled as they are connected through solder jumpers.

The button can serve as a reset button or an interrupt button, the selection is done with solder jumpers.

The DIP-switch shares the same pins as the serial pins and I2C pins, so the I2C port and/or the Bluetooth module cannot be used when the DIP-switch is used.

## Assembly

The assembly of the Robopoly shield is [documented on the Robopoly's website](http://robopoly.epfl.ch/prisme/assemblage).

## Licence

The Robopoly shield is published under [Creative Commons Attribution license](http://creativecommons.org/licenses/by/3.0/).

[![Creative Commons License](http://i.creativecommons.org/l/by/3.0/88x31.png)](http://creativecommons.org/licenses/by/3.0/)
