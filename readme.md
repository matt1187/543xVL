

![grafik](https://github.com/matt1187/543xVL/assets/155289528/43506921-22c4-47fc-8ca6-a63f27ec4e19)


# Project  Cirrus Logic Alpine video card

History: i feel like doing make a underdog-videocard.

![pictures](https://github.com/matt1187/543xVL/blob/main/photo/543xVL_1.jpg)
![pictures](https://github.com/matt1187/543xVL/blob/main/photo/543xVL_2.jpg)
![grafik](https://github.com/user-attachments/assets/5fa25b01-7b75-47cd-9980-3ad1fd9e3056)


# PCB Revision History  
- 543xVL-000 initial draft
- 543xVL-001 few minor bug fixing (wrong config strap and modified RAS0/1 selector)

# Feartures
- Cirrus Logic Alpine (CL-GD5430/5434/5440) video chipset 
- one of very modern video card for VESA local bus platform
- 2 MB DRAM
- 135 MHz integrated RAMDAC (5434)
- rock solid  50 MHz bus-clock with zero wait-state (confirmed since 05.12.2025 on Asus VL/I-486SVGO4x )
- Win 3.1, Win9x, Win NT 3.51 & 4 driver available
- cheap GD5430 PCI card as compoment donor.
- cheap 2 layer platine layout 
- very good VLB bus compatibly (Video card works fine on Alaris Leopard (486SLC2 Motherboard))


  
# Issues 
- GD5430 is not fast, much slower than S3 Trio family.   
- GD5434 isn't easy & cheap find
- some Chip has noisy VGA output (stripe on TFT display)


# notes
- GD5436 hasn't VLB-inteface
- all component with  followed ID is config strap (R1,R2,R3,R4,R5 ,R100,R101 )
- Config strap (R1-5, 100,101 ) Place all resistor except R5
- SPI-EEPROM is optional.
-  5430/5440 ->  RAS0 resistor must be placed,  otherwise  RAS1  resistor must be placed (GD5434)
 

# Bill of material

- [![csv-file ](https://github.com/matt1187/543xVL/blob/main/gerber/543xVL-001.csv)]
- [![Gerber file](https://github.com/matt1187/543xVL/blob/main/gerber/543xVL-001.zip)]

# driver & ROM 
- [![Cirrus Logic ROM generic, from PCI donor card](https://github.com/matt1187/543xVL/blob/main/rom/rom.zip)]







# License
The project is free for non-commercial reproduction. Do not sell it on Ebay or other platforms for profit. Do not make a closed source derivative. Share your experiences and ideas with the community.

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
