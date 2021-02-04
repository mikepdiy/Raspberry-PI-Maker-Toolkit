# Raspberry-PI-Maker-Toolkit
![](pic_rpi_jtag.jpg)
A multi protocol breakout HAT for Raspberry Pi that can work with all the models that have the 40 GPIO making this a versatile HAT for the maker in you plus the cheapest option to get into JTAG, SWDIO , SPI, I2C and UART .<br/>
 I was sick and tired of using expensive brand's to flash my projects under windows and every single time I had to figure out what was wrong. What update was going to crash which part? Will it be the driver ? Maybe one of the softwares in the chain ? So I decied to try and use OpenOCD under linux as the Raspberry Pi is a great candidate to be used as an interface for it. Once I got all working ( on a RPI0W) I never looked back and it is very straight forward to get all working. <\br>
 
 # How to use it ?
 
 1.Jtag and SWD</br>
 For SWD and Jtag I personally used OpenOCD http://openocd.org/ and in order to use ti you have to build it from source . </br>
 A great guide for that was made by Adafruit a while back and can be found here : https://learn.adafruit.com/programming-microcontrollers-using-openocd-on-raspberry-pi </br>
 I have updated the guide a little bit and changed a few small details while making my guide a very simple list of comannds and steps thought I strongly recommned you read first the Adafruit guide as that will explain you the steps done and what they do while my guide is just focused on execution. </br>
 2. SPI</br>
 For SPI I am using Flashrom https://github.com/flashrom/flashrom and I also made a short guide to get that installed and then enable SPI . </br>
 using SPI0 is easy and straight forward and my board has the pinout made for the cheap adapter boards that come with the memory from various online vendors but in order to use SPI1, you have to enable that in the /boot/config.txt file and when you want to jump and use other protocols I suggest to turn it off as some of the pins used by it interffere with the other interfaces. </br>
 SPI0 doesn't have a resistor and capacitor to help with connection issues as they are assumed to pe present on the board that carries the memory ic but SPI1 has them implemented. </br>
 3. I2C </br>
 Here just use use whatever makes you comfortable.</br>
 4. UART </br>
 Again like with I2C just use what you want .</br>
 5. LED Indicator </br>
 The led indicator is present to offer the posibility to give visual feedback of the operations in your scripts. </br>
 
 # Can I use the information without the HAT ? 
 Yes you can and you just need some jumper wires but I made the HAT to aid my work . </br>
 The schematic of the HAT is also available so you can check it out and you can make your own board starting from it .</br>
 
