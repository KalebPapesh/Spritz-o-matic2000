# Spritz-o-matic2000
Motion sensing water sprayer. This has a multitude of uses but it's main purpose was to keep my cats from getting onto the countertops in the kitchen.

# Materials Required
* Arduino
* Power source for Arduino (battery pack or 2A mobile phone charger)
* spritz.ino file
* Servo
* PIR Sensor
* Water bottle with trigger pull sprayer
* Picture hanging wire
* Adjustable metal clamp
* Tape

# Instructions
1. Flash the **Arduino** (or ARM powered device) with _spritz.ino_
2. Attach the **servo** to the **water bottle**  
   This is done by looping the **adjustable metal clamp** around the **servo** and the **water bottle** and tighten  
   **_Note: Do not place the adjustable clamp around the trigger! It should go behind or below the trigger._**
3. Using **picture wire**:  
   1. securely tie one end of it to the part of the servo motor that doesn't move
   2. loop it around the trigger of the **water bottle**
   3. securely tie it to the movable servo head
4. Connect the **PIR sensor** to the front of the water bottle with **tape**  
  **_Note: Do not cover the PIR sensor with tape, use tape around the edges_**
5. Connect the **PIR sensor** to the arduino using:  
    ```bash
   pin 5
    ```
6. Connect the **Servo** to the ardunio using:   
   ```bash
   pin 13
   ```
7. Connect the power source to the **Arduino**
8. Enjoy an cat free countertop!

# What if I have problems?
I've found that the timing between the electronics and the code is quite crucial to successful operation. The spritz.ino has timings for the specific electronics used by me. If you're seeing inconsistent results try adjusting the spritz.ino code to reflect the timing you used.
