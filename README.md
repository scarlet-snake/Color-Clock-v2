# Color-Clock-v2

## Introduction
Clock using my own color-coding systems in place of numbers. It can connect to Wi-Fi and to gets time by NTP and updates a RTC chip to store locally for when it cannot update the time via NTP. There is a photocell at the top to adjust the LED brightness based on ambient brightness. 

## Color System 
I tried to make the system follow 1-3 (RGB), 4-6 (R+G+B), and 7-9 (RGB+W). I did move them around within those patterns to separate similar colors and to suit my own tastes. RGB values provided were selected when viewed through clear PLA and might need to be tweaked for different diffusing material. 

0. White - (255, 255, 255)
1. Red - (255, 0, 0)
2. Blue - (0, 0, 255)
3. Green - (0, 175, 0)
4. Purple - (114, 0, 252)
5. Orange - (250, 107, 0)
6. Yellow - (252, 227, 0)
7. Magenta - (252, 3, 240)
8. Cyan - (3, 248, 252)
9. Light Green - (118, 252, 0)

## Code 
Is mostly an example from the RTC library I used with some modifications. Still need to go through it and clean it up. 

## Case
The case 3d printed from black and clean PLA. I hear that clear PETG might be better than PLA but I have not tried it yet. I printed all the parts without any supports or rafts on my Ender 5. When printing the Shell piece, I set the printer to pause when at the height of 3.2 mm to change from clear to black PLA. 

## Parts
|	Amount	|		Part Type	|		Notes	|
| ------------- | ------------- | ------------- | 					
|1	|photocell|			|
|1	|10kΩ Resistor	|		
|1|330Ω Resistor|	|		|
|1|Screw terminal - 3 pins|	|		|
|1|NodeMCU V1.0	|chip ESP8266; variant NodeMCUV1	|
|1|ZS-042 RTC Module	|chip DS3231; variant 4	|
|1|Prototype Board	|ElectroCookie PCB Prototype Board, Snappable Strip Board with Power Rails|
|10	| M2x6x3.5mm Heat Set Inserts		|I used the cheap ones you buy in a set on amazon and don’t recommend them. You may need to resize the holes for better versions. |
|10	| M2x6 Screws|	|	| |
|.4 meters	|ws2812b LED strip	|30 per meter strip|
## Future/past versions
Version 1 is crude and not worth showing off outside of pictures. I want to take this design and transfer it to custom PCB and cut out all the waste in the nodemcu and RTC module. That is currently out of my ability for the time being.
