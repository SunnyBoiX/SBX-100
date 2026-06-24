# JOURNAL - PROGRESS OF SBX-100 KEYBOARD
## SCHEMATIC
### Layout & Wiring
<img width="1920" height="986" alt="{4D84491C-F9D6-48BA-B200-8252EAB64016}" src="https://github.com/user-attachments/assets/0524c1ef-fa9a-49c0-b99a-b2bb927ec5f3" />
<img width="1919" height="965" alt="{AA4969AA-1894-44A1-ABC2-2E1BE9B552C2}" src="https://github.com/user-attachments/assets/3905b71a-8a34-4c84-afde-2be7f1a87301" />
I originally had a vision of creating a huge keyboard with OLEDs, a rotary encoder, and LEDs, but I realized this would be a struggle during the schematic phase. I originally had a numpad, but I had to remove it because the Raspberry Pi Pico does not have enough GPIO pins, and thus, I wanted to make the keyboard wireless in order to fulfill my happiness. However, this was a terrible idea as well, because wireless microcontrollers, such as nice!nano or nrf types, are really expensive and can also be hard to route during PCB fabrication. I finally made my decision on keeping this project as my learning experience, so if I manage to complete it successfully, I can at least learn the fundamentals on how to make a keyboard, which I can create a new version next time with all the cool stuff I wished for and had to leave out. This keyboard, it is a 100-switch keyboard that also has a rotary encoder switch, and its microcontroller is the Raspberry Pi Pico. I honestly had no idea how to start this project after finding out that a matrix is required for this, so I created one in a different sheet. The main sheet just has the Raspberry Pi Pico and four mounting holes. I connected all the GPIO pins with the global labels I used from the matrix. I disconnected the GPIO pins I didn't need, and still have one GPIO pin left. I'm thinking of adding LEDs, which I might do now. Almost completing this schematic took me over a few days because of how busy I got with events, as it is summer. Overall, my end goal now is to create a 100-switch wired keyboard that has a rotary encoder and LEDs inside of it and is, of course, wired. All I have left to do for the schematic is LEDS now!

### LEDS Complete
<img width="1920" height="972" alt="{4F1F3695-91F1-4220-A073-13B845B7A40C}" src="https://github.com/user-attachments/assets/b92065aa-25d2-4e63-9bf1-04eb9a1fde41" />
<img width="1862" height="958" alt="{8CFCE974-3A7C-4659-BE3B-15D9F1F0AB86}" src="https://github.com/user-attachments/assets/4fdcf950-cc06-413b-8a2f-28826f7714f8" />
I made a separate sheet to work on for the LEDS, and I finally completed the LED stuff. Before doing this, I annotated my schematic to know how many LEDs I would need for each switch. I stored all the LED data in a single global label, and instead of using wires for the next rows, I decided to use Net Labels to make it possible. I completely forgot one crucial step, which is to assign footprints, which I will do now.

### Assigned Footprints
<img width="1920" height="920" alt="{215878CD-280C-480F-8808-A9813762961D}" src="https://github.com/user-attachments/assets/319583c0-88c5-4bdb-ac8e-4e0180efc72f" />
<img width="1920" height="920" alt="{7B05AC75-E501-43FC-8765-99F182B327B2}" src="https://github.com/user-attachments/assets/01d5a6cc-ae95-44df-84fe-51d6881113c3" />
<img width="1919" height="923" alt="{2A39B1DB-C078-4DB0-9210-829FF05B60E9}" src="https://github.com/user-attachments/assets/0abfc4a6-b195-4a9c-8c4b-aa2c5df44fb9" />
<img width="1920" height="922" alt="{7409A7AD-4199-4560-8EF1-C0E76509542A}" src="https://github.com/user-attachments/assets/6fc11443-c1b6-4d59-adfa-d5d8726b0bce" />
I had finally completed assigning the footprints, which I thankfully remembered to do. It was not hard to do because much of it was just MASS assigning the same footprint to the same types of symbols. The only struggle was the mounting holes' footprint. I decided to delete my mounting hole symbols and go with a sandwich mount case style. Now I have successfully completed my schematic and can move on to adjusting the PCB layout and routing!

### COMPLETED SCHEMATIC
<img width="1920" height="991" alt="{E79D0E5F-BF2D-4101-81F3-8AAC820AA03E}" src="https://github.com/user-attachments/assets/e4db5a70-1e2d-4b8b-8faf-26b4de604d38" />
<img width="1920" height="972" alt="{D5856CE4-27C6-405B-9CAA-D73A9B12FC1B}" src="https://github.com/user-attachments/assets/d8ba1482-d2a9-421b-bc7c-3edf613f47c0" />
<img width="1920" height="962" alt="{ECC945BD-C583-4D87-BEB8-AF930303564C}" src="https://github.com/user-attachments/assets/a39aa344-9b76-40a4-80bf-d808a189585f" />

## PCB
