# Hackerboxes0015

All the basic stuff is in the getting-started directory. It's likely a collection of code from all over, it's sometimes unlikely that I recall where I found the code. If headers are in the original code-- they are left intact.

Data and Projects for Hackerboxes 0015

ESP32 DevKitC (ESP-WROOM-32)

	Datasheets
	
		https://espressif.com/sites/default/files/documentation/esp_wroom_32_datasheet_en.pdf

OLED Display 0.96inch 128x64 pixels

	Datasheets
	
	????? appears to be this https://www.youtube.com/watch?v=A9EwJ7M7OsI ????
		
	Helpful Instructables/Videos
	
		http://www.instructables.com/id/Monochrome-096-i2c-OLED-display-with-arduino-SSD13/
		
		http://www.instructables.com/id/How-to-use-OLED-display-arduino-module/
		
		https://www.youtube.com/watch?v=A9EwJ7M7OsI

	Libraries
	
		https://github.com/adafruit/Adafruit_SSD1306
		
		https://github.com/adafruit/Adafruit-GFX-Library
		
	Notes:
		use the i2c scanner library to find your display's address, mine was 0x3C. The code from Arduino Playgraound is in oled-find.ino"

Ring of 24 RGB WS2812 LEDs
	Datasheets
	
		https://cdn-shop.adafruit.com/datasheets/WS2812.pdf
		
	Libraries
	
		Use adafruit NeoPixel for arduino sketches, again from the library with only one modification to the library header made. (comment out the #error line in the header complaining about the height, there is probably a better fix than that-- but it works.)

Matrix Keyboard 4x4

	Datasheets
	
		???? I manually mapped the pins below, just pay attention to the orientation I used while you figure out the pinout.

	Matrix Pin-out
	pins (*Numbered top to bottom, *pins on the left)

			        4*      3*      2*      1*
		|p|  	5*     SW1     SW2     SW3     SW4
		|i|1*					
		|n|2*					
		|s|3*	6*     SW5     SW6     SW7     SW8
		| |4*					
		|h|5*					
		|e|6*	7*     SW9     SW10    SW11    SW12
		|r|7*					
		|e|8*					
		|!|  	8*     SW13    SW14    SW15    SW16
		

Stereo 3.5mm Breakout
	Datasheets
		https://github.com/sparkfun/TRRS_3.5mm_Jack_Breakout


