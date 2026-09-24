# 2v2 Killer Queen
4 player version of arcade game Killer Queen. Custom PCBs for the screen and for each controller. C++ and ARM Assembly Game Engine.
Shared with the official BumbleBear/Killer Queen Team.

## Overview
Designed for embedded systems course. Design goals: multiplayer game, custom sound effects, custom sprites and graphics, Spanish/English toggle. Implemented DAC, ADC, GPIO, UART, button inputs, LEDs.

## Key Results
- Designed schematics and layout for custom PCBs (1 monitor board and 4 controller boards) using Kicad
- Interfaced all PCBs through 12 GPIO pins and UART capability
- Programmed C++ game logic, used structs for custom sprites and sound effects
- Used ARM Assembly for 3 interrupt service routines for button inputs, screen updating, and sound output

## Design
- **PCB System:** Chose to make seperate controller PCBs with input buttons to make 4 player experience easier, monitor board also aggregates all inputs into one screen update 
- **Assembly Interrupts:** Implmented interrupt service routines in assembly for fast input/output processing 
- **Control:** 

## What I'd Change
If I could redo this project, I would put more work into the movement of the sprites. The game engine was functional, but the gameplay was not as fluid as I would have liked which made it less fun. I could have implemented a buffer system for the graphics arrays, so that each update would load faster.

## Media
<img width="450" height="450" alt="image" src="https://github.com/user-attachments/assets/e8d459c3-0781-45d1-b262-1f0da4ff0be7" />
<img width="350" height="450" alt="image" src="https://github.com/user-attachments/assets/601c730b-dadf-4643-9382-e7fc51d69bf8" />


## Tools
C++, ARM Assembly, KiCad, TI MSPM0 Launchpad
