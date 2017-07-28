# LEDBoard_4x4_16bit_HWTest
simple arduino sketch to test the LEDBoard_4x4_16bit PCBs during production

connect one push button to D4 and GND.
Single Click:
toggle sequencer / channel check
hold down: fade to ~100% as long as you push down

as board i used an [Pololu A-Star Mini LV](https://www.pololu.com/docs/0J61/4.1) and a single LiPo-Cell to power it. To have a basic Low-Bat warning i have connected the VIN pin to A0 to measuer Battery Voltage after Polarity Protection (for details see [Schematics](https://www.pololu.com/file/download/a-star-32u4-mini-schematic.pdf?file_id=0J780)) and a red LED to D3.  
The Red LED is switched on if the battery voltage drops below 3.1V.  
in this situation the boards are also switched off and locked.
