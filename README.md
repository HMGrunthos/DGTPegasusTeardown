Repair/teardown of a DGT-Pegasus chess board
===============

* Fault with piece detection on two squares.
* A thin PCB covers the entire play area. 
* PCB is not removable without removing the board surface (polyester sticker?)
* We used heat (clothes iron) to assist in removing it.
* Light pipe array is screwed into the black ABS base at the centre and four corners.
* Rear surface of the PCB holds the control electronics.
* There's a board interface IC, possibly [R5F51303ADFL](https://www.renesas.com/eu/en/products/microcontrollers-microprocessors/rx-32-bit-performance-efficiency-mcus/rx130-cost-optimized-high-performance-32-bit-microcontroller-enhanced-touch-key-function-and-5v-operation)
* Rear surface also holds the LED array, drivers (8x[STP08CP05](https://www.st.com/en/power-management/stp08cp05.html)) and light pipes.
* There are row/column tracks on the front and rear of the PCB running to each square - some kind of inductive piece detection (a short range metal detector?)
* There was a broken track at the end of a row/column leading to inconsistent/missing piece detection.
* Track was repaired and following board calibration (normal process of using the board) seems to work as intended.

Related repository:
https://github.com/EdNekebno/DGTCentaurMods
