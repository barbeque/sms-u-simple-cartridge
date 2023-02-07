# SMS-U Simple
A PCB for Sega Master System games. It's "simple" because it does not include any mapper (page switching, save RAM) logic, which means it only supports most Sega games up to 48K.

Note that this will not work on a Mark III/Japanese Master System; that system's pinout and cartridge shape is totally different.

## Current Status
In development

## Tested With
 * _Snail Maze_ ROM hack

## Bill of Materials
 * PCB
 * (E)EPROM containing your software - 27c64, up to 27c256. 27c512 may work, but only the lower half of the ROM will be accessible.
 * 0.1uF through-hole bypass capacitor

## Assembly Instructions
 1. Submit the gerbers from the Releases page to a PCB fabricator. Suggested settings: gold fingers (ENIG or ideally hard gold,) 45 degree bevel.
 2. If you didn't get edge connector beveling (45-degree fingers) from your PCB fabricator, it may make sense to do the beveling yourself with a sanding block.
 3. Place components onto board. If you are socketing your ROM, the socket may add too much additional height and keep a stock case from fitting.
 4. If you are using a 27c64 for your EPROM (rare,) cut the A14 jumper in the top right of the board and connect the +5V jumper instead. Verify with a multimeter.
