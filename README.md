# Generic electronic candle: remote control commands.
Remote control commands for generic electronic candles.

![image](https://user-images.githubusercontent.com/1586332/129471982-bb24887c-9a95-4a70-8992-64e444fd4dc7.png)

/*

IRremoteESP8266: IRrecvDumpV3 - dump details of IR codes with IRrecv       
An IR detector/demodulator must be connected to the input kRecvPin.        
Copyright 2009 Ken Shirriff, http://arcfn.com       
Copyright 2017-2019 David Conran         
*/

Actual timings from the transmitter:           
![image](https://user-images.githubusercontent.com/1586332/129472069-16994805-5758-40a3-b836-65d92ef408f2.png)
https://codepen.io/SarahC/pen/VwbNMwR?editors=0010        


Generic electronic candles - remote control.          

IRrecvDump is now running and waiting for IR input on Pin 36      
Library : v2.7.19      
Protocol : NEC       

Key : On       
Code      : 0xFF00FF (32 Bits)       
uint16_t rawData[71] = {9034, 4494,  604, 558,  502, 634,  546, 562,  552, 582,  502, 634,  552, 558,  576, 560,  500, 634,  550, 1666,  530, 1714,  602, 1672,  580, 1666,  480, 1764,  580, 1694,  578, 1668,  524, 1718,  606, 558,  502, 632,  516, 594,  546, 588,  502, 608,  576, 558,  580, 556,  498, 636,  518, 1702,  528, 1716,  604, 1666,  578, 1668,  528, 1716,  576, 1696,  578, 1666,  530, 1714,  606, 39980,  9064, 2218,  528};  // NEC FF00FF       
uint64_t data = 0xFF00FF;       
       
Key : Off       
Code      : 0xFF807F (32 Bits)       
uint16_t rawData[71] = {9020, 4506,  564, 598,  510, 598,  536, 598,  536, 598,  512, 598,  536, 598,  534, 600,  510, 600,  538, 1708,  536, 1708,  562, 1682,  566, 1706,  538, 1708,  558, 1686,  564, 1708,  536, 1710,  560, 1682,  566, 596,  536, 600,  512, 596,  538, 598,  536, 600,  510, 598,  538, 596,  534, 600,  510, 1710,  562, 1684,  562, 1708,  538, 1708,  560, 1684,  562, 1710,  536, 1708,  562, 40024,  9020, 2262,  512};  // NEC FF807F       
uint32_t address = 0x0;       
uint32_t command = 0x1;       
uint64_t data = 0xFF807F;       
       
Key : 4 Hours       
Code      : 0xFF40BF (32 Bits)       
uint16_t rawData[67] = {9018, 4510,  556, 608,  524, 584,  550, 584,  498, 636,  524, 586,  550, 586,  502, 608,  574, 560,  548, 1696,  550, 1694,  528, 1714,  576, 1698,  552, 1692,  526, 1720,  578, 1694,  574, 1670,  528, 632,  550, 1668,  528, 634,  526, 584,  550, 586,  502, 634,  550, 558,  578, 558,  502, 1714,  604, 560,  500, 1716,  580, 1694,  550, 1698,  526, 1716,  602, 1670,  576, 1668,  528};  // NEC FF40BF       
uint32_t address = 0x0;       
uint32_t command = 0x2;       
uint64_t data = 0xFF40BF;       
       
Key : 8 Hours       
Code      : 0xFFC03F (32 Bits)       
uint16_t rawData[71] = {9016, 4512,  530, 632,  526, 584,  548, 588,  500, 634,  524, 586,  550, 584,  502, 632,  550, 560,  574, 1668,  578, 1668,  532, 1712,  580, 1694,  552, 1694,  526, 1716,  580, 1694,  576, 1672,  524, 1716,  578, 1694,  574, 562,  574, 562,  502, 632,  550, 558,  574, 560,  500, 634,  524, 586,  576, 558,  500, 1718,  576, 1694,  552, 1692,  530, 1716,  602, 1668,  552, 1692,  530, 40056,  9014, 2266,  544};  // NEC FFC03F       
uint32_t address = 0x0;       
uint32_t command = 0x3;       
uint64_t data = 0xFFC03F;       
       
Key : Candle mode       
Code      : 0xFF20DF (32 Bits)       
uint16_t rawData[71] = {8996, 4530,  538, 598,  540, 596,  508, 628,  512, 596,  538, 596,  534, 602,  512, 596,  540, 596,  530, 1690,  564, 1708,  512, 1756,  508, 1712,  566, 1706,  538, 1706,  558, 1686,  564, 1708,  512, 622,  540, 596,  506, 1714,  540, 620,  506, 630,  516, 594,  540, 594,  532, 604,  516, 1706,  556, 1686,  568, 594,  504, 1714,  568, 1702,  542, 1704,  528, 1716,  570, 1702,  542, 40042,  9008, 2248,  600};  // NEC FF20DF       
uint32_t address = 0x0;       
uint32_t command = 0x4;       
uint64_t data = 0xFF20DF;       
       
Key : Light mode       
Code      : 0xFFA05F (32 Bits)       
uint16_t rawData[71] = {9006, 4522,  550, 586,  550, 586,  500, 634,  524, 586,  548, 588,  502, 632,  550, 558,  576, 558,  502, 1718,  604, 1668,  574, 1670,  530, 1716,  604, 1668,  542, 1702,  530, 1714,  600, 1672,  576, 1670,  528, 634,  524, 1696,  528, 608,  550, 584,  552, 584,  500, 608,  544, 592,  576, 560,  502, 1716,  602, 560,  500, 1718,  578, 1694,  578, 1668,  528, 1714,  602, 1670,  548, 40036,  8996, 2260,  562};  // NEC FFA05F       
uint32_t address = 0x0;       
uint32_t command = 0x5;       
uint64_t data = 0xFFA05F;       

Key : Dimer       
Code      : 0xFF906F (32 Bits)       
uint16_t rawData[71] = {9000, 4528,  542, 594,  540, 594,  506, 630,  516, 592,  540, 596,  530, 606,  516, 594,  540, 594,  530, 1688,  568, 1704,  542, 1702,  530, 1716,  568, 1702,  544, 1704,  530, 1714,  570, 1702,  542, 1704,  558, 604,  518, 592,  544, 1702,  542, 594,  542, 592,  530, 606,  516, 592,  540, 594,  504, 1714,  570, 1700,  544, 592,  546, 1700,  546, 1702,  526, 1716,  574, 1700,  544, 40040,  9034, 2220,  602};  // NEC FF906F       
uint32_t address = 0x0;       
uint32_t command = 0x9;       
uint64_t data = 0xFF906F;       
       
Key : Brighter       
Code      : 0xFFE01F (32 Bits)       
uint16_t rawData[67] = {9006, 4522,  544, 590,  546, 590,  500, 634,  520, 590,  546, 588,  530, 606,  522, 588,  570, 564,  500, 1718,  574, 1698,  546, 1700,  528, 1716,  576, 1696,  546, 1698,  556, 1688,  574, 1700,  546, 1696,  556, 1690,  574, 1698,  546, 588,  546, 590,  504, 632,  520, 590,  544, 590,  504, 630,  518, 590,  544, 592,  502, 1716,  570, 1704,  544, 1702,  556, 1688,  568, 1706,  538};  // NEC FFE01F       
uint32_t address = 0x0;       
uint32_t command = 0x7;       
uint64_t data = 0xFFE01F;       



