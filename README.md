<img width="130" height="288" alt="WhatsApp Image 2026-05-28 at 11 33 49 PM" src="https://github.com/user-attachments/assets/55b05c16-0c3c-446d-884e-c3197c893ac6" />


Hey! I have built a simple lyrics karoake project where I stored lyrics and display them at specific time stamps (just like a karoake video). 

Components Used:
1. Arduino Uno- Main processor 
2. 16x2 LCD screen- For displaying the results
3. I2C backpack adapter- Helped me to reduce the amount of connections into total 4 wires (VCC, GND, SDA and SCL)
4. USB cables- For sending codes to the arduino

The main issue I faced while storing lyrics was that Arduino UNO had a fixed small SRAM of 2KB, so it couldnt store much of the lyrics. 
Then I found out we could use the 32 KB flash memory also where usually code is stored.

Connections-
1. VCC of I2C - 5V of arduino
2. GND of I2C - GND of arduino
3. SDA of I2C - A4 of arduino
4. SCL of I2C - A5 of arduino

Libraries-
1. Wire.h
2. LiquidCrystal_I2C.h
