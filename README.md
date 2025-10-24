# Custom Ergonomic Keyboard Project

This repository contains the design files, firmware, and documentation for a custom ergonomic mechanical stenography keyboard. The keyboard features a compact layout with 36 keys found on a standard full-size keyboard. I will be using a custom QMK firmware for the keyboard, which will be available in the `firmware/` directory.

# Final Goal Layout

The Layout I used called [Haori36](https://github.com/penk/Haori36) by penk. It is a 36-key layout that includes all the essential keys found on a standard full-size keyboard, arranged in an ergonomic manner to reduce finger travel and increase typing efficiency. 

Traditional stenography keyboards have a unique layout that allows for chorded key presses, enabling users to type entire words or phrases with a single hand motion. This layout is designed to facilitate such chorded inputs while maintaining a compact form factor. A standard stenography layout typically have 24 keys, but I will make use of the FN layer to turn it into a traditional QWERTY layout when needed.

![Final Format](/docs/image.png)

# Case and Plate Design

The case and plate for the keyboard was designed by penk; however, I will be making some modifications to better suit my preferences and needs. The design files will be available in the `case/` and `plate/` directories respectively of the `model` folder. I will later use Fusion 360 to refine the case design and prepare it for 3D printing or CNC machining.

# PCB

I used the standard PCB design provided by penk for the Haori36 layout. The PCB files will be available in the `pcb/` directory. I will make sure to review the PCB design and make any necessary adjustments to ensure compatibility with my chosen components and layout modifications. I will be using JCLPCB to fabricate the PCB, also their assembly service to solder the SMD components. This will save me time and effort compared to hand-soldering the diodes myself.

# BOM 
The Bill of Materials (BOM) for the keyboard project is as follows:

Quantity | Item | source
--- | --- | ---
1 | RP2040-Zero & Pin headers | [RP2040](https://www.amazon.com/dp/B09KZPCNPL) and [Pin](https://www.amazon.com/dp/B0817JG3XN)
1 | Haori36 PCB | [Penk's GitHub](https://github.com/penk/Haori36)
1 | Haori36 plate | [Penk's GitHub](https://github.com/penk/Haori36)
36 | Kailh Choc V1 switches | [Kailh](https://www.kailhswitches.com/)
36 | Kailh Choc V1 Hot-swap sockets | [Kailh](https://www.kailhswitches.com/)
36 | 1N4148 diodes (SMD) | JCLPCB assembly service
4 | M2x4 heat-set thread inserts | [Amazon](https://www.amazon.com/dp/B0DQL44Z2V)
4 | M2x6 screws | [Amazon](https://www.amazon.com/dp/B0CMCTX529)

These were given by penk in his original project, and I will source them from various electronics suppliers and online retailers.

# Firmware

I will be using QMK firmware for the keyboard, which will be customized to support the Haori36 layout and any additional features I wish to implement. The firmware files will be available in the `firmware/` directory. I will ensure that the firmware is properly configured to work with the RP2040-Zero microcontroller and the specific key mapping of the keyboard.`
