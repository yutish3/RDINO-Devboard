# Journal 1 ( 2 HOURS ) :- initial planing 

the idea is the same as description
things i have decided :-

    it will use rp2040
    16 Mbit flash memory for extra ram (16 mega bit is 4mb )
    bluetooth module (the one used in esp32)
    5x5 neo pixel led grid (coz it looks cool ngl)
    usb c for programing

i selected all the components for each thing all the things i mentioned above and for voltage regulation and got them all into kicad and arranged them into a decent manner also studied arduino uno shape and headers location it has 2 8 and 2 6 female header chains

<img width="1414" height="964" alt="image" src="https://github.com/user-attachments/assets/ed676e51-46a8-4c56-8d71-7037a7e0fe91" />

---

# Journal 2 ( 1.5 HOURS ) :- made schematic of power system 

so how this power system works is the whole board works on usb c and from usb c the power goes to AP2112K-3.3 which converts the 5v into 3.3v which we will use to power almost the entire board except neo pixels which require 5v so for them i will connect them directly to VBUS(5V) instead of VCC(3.3V) and the crystal oscilator is used for syncronising the rp2040 chip to other signals i also placed the power and gnd flags in start i learned it from my last project 

<img width="664" height="1330" alt="image" src="https://github.com/user-attachments/assets/7e1d129d-7de5-45fc-8997-535d965dacee" />

---



