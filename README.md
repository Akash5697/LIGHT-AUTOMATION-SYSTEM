# LIGHT-AUTOMATION-SYSTEM
I have done Light Automation System and my main objective is to save Energy. By this project, i am reducing the amount of time, a bulb used thus reducing electricity bill. 

PROJECT COMPONENT LIST
1. Arduino uno
2. Breadboard
3. LED
4. Resistor
5. PIR Sensor
6. LDR 
7. Jumper Wire

DESCRIPTION OF EACH COMPONENT
⮚	Arduino uno : Arduino Uno is a microcontroller board based on the ATmega328P (datasheet). It has 14 digital input/output pins (of which 6 can be used as PWM outputs), 6 analog inputs, a 16 MHz ceramic resonator (CSTCE16M0V53-R0), a USB connection, a power jack, an ICSP header and a reset button. 

⮚	BreadBoard  : A breadboard is a solderless device for temporary prototype with electronics and test circuit designs. Most electronic components in electronic circuits can be interconnected by inserting their leads or terminals into the holes and then making connections through wires where appropriate

⮚	LED : A light-emitting diode (LED) is a semiconductor light source that emits light when current flows through it. Electrons in the semiconductor recombine with electron holes, releasing energy in the form of photons. The color of the light (corresponding to the energy of the photons) is determined by the energy required for electrons to cross the band gap of the semiconductor. White light is obtained by using multiple semiconductors or a layer of light-emitting phosphor on the semiconductor device.

⮚	Resistor: A resistor is a passive two-terminal electrical component that implements electrical resistance as a circuit element. In electronic circuits, resistors are used to reduce current flow, adjust signal levels, to divide voltages, bias active elements, and terminate transmission lines, among other uses. 

⮚	PIR Sensors: A passive infrared sensor (PIR sensor) is an electronic sensor that measures infrared (IR) light radiating from objects in its field of view. They are most often used in PIR-based motion detectors. PIR sensors are commonly used in security alarms and automatic lighting applications. 

⮚	LDR : A photoresistor (also known as a light-dependent resistor, LDR, or photo-conductive cell) is a passive component that decreases resistance with respect to receiving luminosity (light) on the component's sensitive surface. The resistance of a photoresistor decreases with increase in incident light intensity; in other words, it exhibits photoconductivity. A photoresistor can be applied in light-sensitive detector circuits

⮚	Jumper Wire: Jumper cables is a smaller and more bendable corrugated cable which is used to connect antennas and other components to network cabling.

PROJECT DISCUSSION :-

My project counts the number of people entering and exiting the room. Using two PIR sensors, side by side sensors, we created a SINGLE DOOR COUNTER. When a person enters a room, our counter count adds 1. If a person exits the room, the counter subtracts 1. By doing this, it can determine the people present in the room. I am also using a ldr sensor for detecting light intensity. If none of the people is greater than one and the light intensity is below the selected threshold intensity, then the light will be turned on. If people are present, but the light intensity is above the threshold, then lights will not be turned on. If the light intensity is below the selected threshold, but there are no people in the room, the lights will be turned off.

METHODOLOGY
●	Input pin of 1st pir sensor connected to arduino digital port 5. Gnd  and vcc pin connected to gnd and vcc of arduino using breadboard.
●	 Input pin of 2nd  pir sensor connected to arduino digital port 6. Gnd  and Vin pin connected to gnd and vcc of arduino using breadboard.
●	LDR one pin connected to Vcc and othe pin is connected to analog pin A0 and gnd using 1k resistor
●	Green, Red, Blue led input pins are connected to digital port 2 ,3 ,4 respectively. Their output pin is connected to gnd using resistors.
●	When one person entered the room the no of people is one. Now ldr reading is lesser than threshold value. So lights are turned on. Now another person entered the room. So no of people becomes 2. So light is still on. 
●	Now two person exit the room one by one. So no of people is zero. So light is turned off though ldr reading is greater than threshold. 
●	If  person is present in the room but light intensity is more than threshold light will turned off

