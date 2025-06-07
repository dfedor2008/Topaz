---
title: "Topaz"
author: "Dawid Fedor"
description: "Radio module which can pressure, temperature and humitidy, and location"
created_at: "2025-05-27"
---
Total time: 4.5h
Day 1:
Today I worked on the schematic. I decided to use a SAMD21, an SX1262, and a BME280, as I have previous experience with them. I imported custom parts from Snap EDA and modified the (PE4257, and ESC32TXO).
Time spent:~2 hours
![image](https://github.com/user-attachments/assets/426dea85-c6ab-4282-aeb5-567c2c0c2165)


Day 2:
The schematic is finished. I moved on to the PCB layout. I imported a custom oscillator (ECS-327TXO-2012) for the SAMD21. I'm quite happy with the design so far.
I also revisited the schematic and added another button, which could potentially be used for Morse code input in the future.
Time spent:~1.5 hours

Day 3:
I changed the minimum track spacing to 0.127 mm to prevent copper pads from merging, in line with OSH Park’s manufacturing limits.
I also worked on minimizing the PCB size to help reduce production costs.
Time spent:~1.75 hours

Day 4:
Final changes were added. Fixed certain errors in DRC. Fixed final arragment problems. I went back to KiCad and ran ERC to checked and fixed any errors.
I reviewed for a final time the schematic to see if I missed anything ( compared it with the manufactorers reference design and datasheets). 
Time spent: 1.25 hours
![image](https://github.com/user-attachments/assets/9d6ee133-5bca-4c68-a8b3-d9f310b69f3c)

Day 5:
I added a GPS module so that location can be transmitted. I added a ATGM336H, which is a very cheap module.
![image](https://github.com/user-attachments/assets/5953250e-d070-40ac-8189-2106e2e3f7e4)



Overall Notes:
The biggest challenge I faced was figuring out the RF section. The manufacturer-recommended RF switch, the BGS12WN6E6327, is extremely small and nearly impossible to solder by hand.
To resolve this, I decided to find a replacement and settled on the PE4259, which is considerably larger and easier to solder.
