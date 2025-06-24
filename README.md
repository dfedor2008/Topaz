                                                                            Topaz

Topaz is a PCB which uses a SX1262 radio to send morse code up to 13 km. It can also be used to send temperature :).
The microcontroller is a SAMD21 which is a great microcontroller which I used because of my previous experience with it.
The barometric pressure sensor is a BME 280. It is a cheap and reliable pressure, temperature, and humidity sensor.


Application notes:

After getting the PCB you should begin by soldering it. If you have a heating plate, then I would use it for sure.
After soldering check for shorts and plug in the PCB (not to your computer) . If you see smoke, imedaitly unplug the
pcb and check for shorts. If there are no shorts then plug it into your computer. The code will be uploaded after I assemble the PCB.
The whole PCB is made so that it can be cheap and reliable.

Why I made this project:

I made this project because I wanted to make a GPS tracker which I could use to track my bus ( which is often very late). 
I would also like to use it to track brother while playing hide and seek ( a practical joke). This project however as a lot
of other possible applications with tracking and sending data.

How someone can use it:
Topaz is a versatile GPS tracker designed to transmit real-time telemetry data over radio. Whether you're keeping track of hikers to ensure no one gets lost, or recovering a high-flying rocket after launch, Topaz provides reliable location tracking without relying on cellular networks. Its flexible design makes it suitable for a wide range of applications based on what you are trying to achieve.

How it works:
Topaz uses the ATGM336H GPS module to collect positioning and telemetry data. This data is then processed by the SAMD21 microcontroller, which handles communication and control logic. The processed data is transmitted via the SX1262 radio module, which functions as both a transmitter and a receiver. This enables two Topaz devices to communicate with each other. All code will be writted in C++ due to the libraries for these sensors are very reliable.

PCB Schematic:
![image](https://github.com/user-attachments/assets/f2879cd7-5488-43de-9e77-05d04c68f9a8)


PCB Layout:
![image](https://github.com/user-attachments/assets/378aa5f3-1122-452e-8baf-344f799cf8b8)





