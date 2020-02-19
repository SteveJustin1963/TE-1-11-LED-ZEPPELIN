# TE-1-11-LED-ZEPPELIN

https://easyeda.com/editor#id=bbd7b8d58a2d43f18a62c44de48721b0|e61d4ab7e8414d7b9a3737383128992b

Led Zeppelin is a game of patience. It's like getting a kite into the air. It goes up slowly but the slightest mistake will bring it down like a lead balloon. 

![](https://github.com/SteveJustin1963/TE-1-11-LED-ZEPPELIN/blob/master/ledzep-cct.png)

## Our game name,LED ZEPPELIN, is a play on words:
It comes not from the pop group but from Graf Von Zeppelin, a german army officer who invented the first rigid air ship in 1900. The association fits perfectly with this project. The game consists of six LEDs which flash at 2 cycles per second. A push button is the "Operations Control" and by carefully pushing the button in synchronization with the flashes, the row of LEDs will gradually light up but the slightest mistake will immediately extinguish one, two or three LEDs.  
## HOW THE CIRCUIT WORKS 
The circuit consists of a three-inverter CMOS clock oscillator driving Q8 which flashes the LEDs on and off. The other output from the oscillator is used to charge up the 470mfd electrolytic C2, via R3. The output from pin 3 is in the form of a square wave only slightly less than the supply voltage and is about 7.5v to 8v. The frequency of oscillation is governed by R1 , R2and C1 and is approximately 2Hz. Charging of the 470mfd electrolytic is exponential so that initially the voltage increments on the capacitor will be greatest when it is beginning to charge. Each time the button is pressed a small amount of energy is fed into C2. This voltage appears at the base of Qi which is connected as an emitter-follower and the voltage will appear proportionally at the emitter, less the .6v base-emitter voltage drop of Q1. This voltage is then fed to the base of six transistors Q2 to Q7 which drive LEDs 1-6 via current limiting resistors. Each of these transistors will turn on according to the voltage on the 470mfd electrolytic. As the voltage rises to .6v, Q1will turn on. For Q2 to turn on its base must be .6v highet than the emitter. Now Q2 has a forward-biased diode in its emitter lead and the voltage drop across it will be .6v. The base of Q2must be .6v above the emitter, making it .6 plus .6 or 1.2v This means the voltage on C2will be .6v plus .6v plus .6v or 1.8v for the first LED to be fully lit. The emitter of Q3 is connected to the base of Q2so that a further .6v will turn it on. At each successive .6v rise the next transistor in the chain will turn on until finally Q7 will switch on. This transistor drives the top LED which is the highlight of the game. When you have LED 6 pulsating you really feel a sense of achievement. Should the button be pressed when the oscillator is low, the diode D1is forward biased and the charge on C2 will rapidly discharge through R4. Since the voltage increments become smaller as the 470mfd becomes fully charged, to light the top LED requires significantly more pushes than LEDs 1 and 2. If, however, the button is pushed too long, the discharge will be greatest when the capacitor is nearing full charge and an error here will lose the gain made by many pushes. This is where the skill of the game comes in. The charging of the capacitor is "out of phase" with the flashing of the LEDs. This means the button must be pressed when the LEDs are extinguished. To turn the game off, push the button when the LEDs are lit. This will remove the charge on C2and eventually every LED will go out.

## CONSTRUCTION
All the components are mounted on the Printed Circuit Board. Follow the layout diagram for the identification of each part. You will notice all the components are placed neatly on the board with Q2 - Q7 fitted the same way around and all LEDs mounted the same way. For the transistors a dot on the PC board signifies the collector lead. Both electrolytics are identified with their positive lead. The IC has pin 1 shown and the switch connections are also identified. 

## PARTS LIST
* R1 470k
* R2 56k
* R3 22k
* R4 47OR
* R5 4k7
* R6 3k3
* R7 2k2
* R8 2k2
* R9 1k
* R10 1k
* R11 56OR 
* R12 47OR 
* R13 47OR 
* R14 390R
* R15 330R 
* R16 27OR 
* R17 10k
* R18 1k
* Cl electrolytic 4.7mfd 16v
* C2 47Omfd 16v
* Q1 - Q7 transistors BC 547
* Q8 BC 557
* IC1 CD 4001
* LED1 - LED6 Large Red LEDs
* LED7 miniature red Light Emitting Diode
* D1 D2 diodes 1N914 or IN 4148
* Sw1 push button
* battery clip
* 9v battery
* "Led Zeppelin" PC Board 

