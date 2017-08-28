

## STM32F103C8 Black Pill ( PB12) 

Serialport set and display RTC clock , Writer: CSNOL  https://github.com/csnol/STM32-Examples
based on https://github.com/rogerclarkmelbourne/Arduino_STM32

1. Blink on PB12 per 1s. 
2. change to your timezone in the sketch; . 
3. get Unix epoch time from https://www.epochconverter.com/ ; 
4. last step input the 10 bits number( example: 1503945555) to Serialport ;
5. the clock will be reset to you wanted.

##  Why the 10 bits Unix epoch time be used?
#### Because I wanna connect to NTP server by ESP-8266. 
#### in the <NTPClient.h> library. getNtpTime() will return this 10 bits Unix epoch time.
