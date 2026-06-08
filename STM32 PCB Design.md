<img width="1612" height="886" alt="image" src="https://github.com/user-attachments/assets/8dc18c00-a72c-4029-86aa-f34d8488bb01" />


<img width="800" height="584" alt="image" src="https://github.com/user-attachments/assets/9b3c5ba9-6541-44fb-b256-3c4f581d499f" />


This is a custom STM32 microcontroller breakout board that I designed from scratch using KiCad. The whole project started with drawing the schematic layout where I wired up an AMS1111 linear voltage regulator to safely drop the incoming USB power down to a stable 3.3 volts. I also added a status indicator LED to let me know whenever the board is actually getting power. For the main microcontroller, I included crucial supporting parts like a 16 megahertz crystal oscillator for accurate timing, a physical boot toggle switch, and a handful of decoupling capacitors placed right next to the power pins to filter out electrical noise.

After finishing the circuit schematic, I transitioned over to the PCB editor to route the actual physical board layout. I went with a compact four layer board design using internal ground and power planes to keep the signals incredibly clean. I paid close attention to part placement, keeping the crystal oscillator traces as short and symmetrical as possible to avoid signal interference. I broke out all the primary communication protocols to dedicated pin headers along the edges, including labels for UART, I2C, and SWD debug testing. I even added custom mounting holes on all four corners so I can easily secure the board into a 3D printed case or project enclosure later on.
