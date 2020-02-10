# Colour-Sensor

The colour sensor is made using the following components: LDR, LEDs and arduino.

The LDR is useful for detecting the brightness of light. The light with more intensity reduces the resistance within the LDR and vice versa.
The three LEDs of colours red, green and blue, blink one after another on an object whose colour is desired.
The object reflects most of the light of its own colour and absorbs the rest. This reflected light is directed to the LDR sensor.
So the LDR shows least resistance (declares highest brightness) when the LED that is of the same (or similar) colour as the object glows,
as it reflects most of its light.
For example, if a green object is placed in front of the LDR, the resistance of the LDR is high when red or blue LEDs glow on it, whereas
the resistance becomes minimum when the green LED glows.
This is the principle used to convert a brightness sensor (LDR) to a colour sensor.

The arduino is used for decoding the data LDR senses in the form of the voltage across it. It drops higher voltage when it exhibits 
larger resistance. This voltage value is taken for each case where each of the red, green and blue LEDs shine on the object and is compared
in the software of arduino, in order to return the output colour.
