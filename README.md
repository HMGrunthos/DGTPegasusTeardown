# Repair/teardown of [DGT's Pegasus](https://digitalgametechnology.com/products/home-use-e-boards/dgt-pegasus) online chess board

> We believe that the play area/sensor PCB may be shared with [DGT's Centaur](https://digitalgametechnology.com/products/chess-computers/dgt-centaur-chess-computer)

## Fault:
Inconsistent piece detection (absent and spurious) on two squares.

## Teardown & fix
* A thin board/sensor PCB covers the [entire play area](Pictures/DGT_Pegasus_BoardExposed.jpeg).
* The power/interface PCB is connected to the board/sensor PCB by a ribbon cable.
* The board/sensor PCB is not accessible without delaminating the [board surface](Pictures/TopSticker_Removed-2.jpg) (a polyester sticker?)
* We used heat (a clothes iron) to assist in removing it (the board surface.) 
* A [light pipe array](Pictures/LightPipeArray-4.jpg) (polycarbonate?) is screwed into the black [plastic ABS base](Pictures/ABSBase-1.jpg) at the centre and four corners (screws inaccessible without removing the board surface.
* The rear surface of the board/sensor PCB holds the play area [control electronics](Pictures/PCB-BottomLEDsAndControl-ControllerDetail-1.jpg).
* There's an IC on the rear surface of the board/sensor PCB (part of the control electronics, acting as a sensor interface?) Possibly [R5F51303ADFL](https://www.renesas.com/eu/en/products/microcontrollers-microprocessors/rx-32-bit-performance-efficiency-mcus/rx130-cost-optimized-high-performance-32-bit-microcontroller-enhanced-touch-key-function-and-5v-operation)
* The [rear surface](Pictures/PCB-BottomLEDsAndControl-WholeBoard-1.jpg) of the board/sensor PCB also holds the LED array, LED drivers (8x[STP08CP05](https://www.st.com/en/power-management/stp08cp05.html)) and interfaces to the light pipes (to bring the LED light output to the board surface.)
* There are row/column tracks on the front and rear of the PCB [running to each square](Pictures/PCB-TopDetectors-TrackDetail.jpg) - inductive piece detection (essentially a short range metal detector?)
* There was a broken track at the end of a row/column leading to inconsistent/missing piece detection.
* The faulty PCB track was repaired, and following board calibration (a normal process of using the board) the board seems to work as intended.

## Related repositories:
https://github.com/EdNekebno/DGTCentaurMods
