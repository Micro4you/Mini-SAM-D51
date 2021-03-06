# Mini SAM D51
Mini SAM D51 is a LEGO® minifigure-sized development board based on the Microchip SAMD51G 48-Pin 32-Bit ARM® Cortex®-M4F MCU running at 120Mhz.  If you are familiar with some other of my minifigure-sized boards, you'll notice I managed to create this one in a 2-layer format, which saves us money.

## On-board Features


### I/O
The board includes a usb-micro interface for programming and power.   Around the edge are 0.050" spaced holes and the plan is to have a "breakout" board with standard .100" headers.  In addition, future revisions will have castellated holes.  Still working through the design.

Mini SAM D51 includes two LED indicators; a standard Arduino "Built-In" LED and an APA102 RGB LED - useful for [CircuitPython](https://github.com/adafruit/circuitpython) - and available for programming in Arduino as well.  There are two built-in buttons as well; a RESET button and a user programmable BUTTON.

### Memory
In order to support CircuitPython, a 2MB Quad-SPI flash memory chip is included.  This provides plenty of space for the CircuitPython program as well as space for user programming.

### Other
The board includes a 600mA 3.3V regulator, more than enough to power this little board and its built-in features.  The micro-USB circuitry includes optional provisioning for case grounding and ESD protection.  Finally, The AREF input and recommended Analog and Digital power separation is present on the board.

## BOM
[Github linked BOM](https://github.com/bwshockley/Mini-SAM-D51/blob/master/BOM/SAMD51-007) includes everything required to fully populate the board.  Please note the optional items in the schematic on Github.

## Arduino
Arduino FIRMWARE/BOOTLOADER is **in-work**. The goal is a bootloader that has all functions working and all on-board features usable with "Built-In" terminology in Arduino, i.e. LED_BUILTIN, MOSI, MISO, SCK, and BUTTON_BUILTIN.

## CircuitPython
CircuitPython work is **in-work** and will utilize the wonderful work done for the [Adafruit ItsyBitsy M4](https://www.adafruit.com/product/3800) - as it is essentially the same board.

Bootloader for Mini SAM M4 can be built from this source: [UF2-SAMDX1](https://github.com/bwshockley/uf2-samdx1) 

## Open Source
Boards can be ordered direct from [OSHPark](https://oshpark.com/profiles/bwshockley).
