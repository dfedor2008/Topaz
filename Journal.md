---
title: "Topaz"
author: "Dawid Fedor"
description: "Radio module which can send morse code or pressure, temperature and humitidy"
created_at: "2025-05-28"
---

Day 1:
Today I worked on the schematic. I decided to use a SAMD21, an SX1262, and a BME280, as I have previous experience with them.

Day 2:
The schematic is finished. I moved on to the PCB layout. I imported a custom oscillator (ECS-327TXO-2012) for the SAMD21. I'm quite happy with the design so far.
I also revisited the schematic and added another button, which could potentially be used for Morse code input in the future.

Day 3:
I changed the minimum track spacing to 0.127 mm to prevent copper pads from merging, in line with OSH Park’s manufacturing limits.
I also worked on minimizing the PCB size to help reduce production costs.

Overall Notes:
The biggest challenge I faced was figuring out the RF section. The manufacturer-recommended RF switch, the BGS12WN6E6327, is extremely small and nearly impossible to solder by hand.
To resolve this, I decided to find a replacement and settled on the PE4259, which is considerably larger and easier to solder.
