# pinball-scoring

Screen: Adafruit 2050 TFTLCD, did not use touchscreen capabilities
Board: Arduino Uno

To use this screen, there are a few things that you need to do in order for it to work as intended. If using SPI communication to the board, you need to solder the IM2 jumper on the back of the board, OR you need to jump the IM2 pin to the 3Vo pin. 
*********************** DO NOT TIE IT TO 5 VOLTS!!!!!!!!!! ************************************

This picture shows the solder jumper on the back of the board
![IMG_2726](https://github.com/jbowens130/pinball-scoring/assets/158515070/776a726d-3063-467e-81fe-6541a9cb9f8f)

Pin assignments: 
3-5V: 5V
CLK: Arduino 13
MISO: Arduino 12
MOSI: Arduino 11
CS: Ardino 10
CD: Arduino 9
RST: Arduino 8

CS,CD and RST can be changed in software, they are flexible.

You will need adafruit libraries to communicate with the board, and for graphics. All libraries can be downloaded in the Arduino IDE through manage libraries. Check the wiki page "Library Installation" for details.
For SPI communication to board you need the Adafruit_HX8375D library 
For graphics, you need the Adafruit_GFX library

