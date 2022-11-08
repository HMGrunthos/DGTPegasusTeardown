Repair/teardown of [DGT's Pegasus](https://digitalgametechnology.com/products/home-use-e-boards/dgt-pegasus) online chess board
===============

Fault: Inconsistent piece detection (absent and spurious) on two squares.

* A thin board/sensor PCB covers the entire play area.
* The board/sensor PCB is not removable without delaminating the board surface (a polyester sticker?)
* We used heat (a clothes iron) to assist in removing it (the board surface.)
* The power/interface PCB is connected to the board/sensor PCB with a ribbon cable. 
* A light pipe array is screwed into the black ABS base at the centre and four corners (screws inaccessible without removing the board surface.)
* The rear surface of the PCB holds the play area control electronics.
* There's a board interface IC on the rear surface, possibly [R5F51303ADFL](https://www.renesas.com/eu/en/products/microcontrollers-microprocessors/rx-32-bit-performance-efficiency-mcus/rx130-cost-optimized-high-performance-32-bit-microcontroller-enhanced-touch-key-function-and-5v-operation)
* The rear surface also holds the LED array, drivers (8x[STP08CP05](https://www.st.com/en/power-management/stp08cp05.html)) and light pipes.
* There are row/column tracks on the front and rear of the PCB running to each square - inductive piece detection (essentially a short range metal detector?)
* There was a broken track at the end of a row/column leading to inconsistent/missing piece detection.
* The faulty PCB track was repaired, and following board calibration (normal process of using the board) seems to work as intended.

Related repository:
https://github.com/EdNekebno/DGTCentaurMods
