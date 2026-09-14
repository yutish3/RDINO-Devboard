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

# Journal 3 ( 0.4 HOURS ) :- completed the wiring for buttons and esp 32 wifi 

completed the wiring esp 32 wifi and 2 buttons 1 for reset the board and 1 for running the board which completes a major part of the schematic process

<img width="744" height="688" alt="image" src="https://github.com/user-attachments/assets/997a7f2b-05b3-4b23-a8c6-1265a1ad8f55" />
<img width="1234" height="652" alt="image" src="https://github.com/user-attachments/assets/63476427-d48d-4899-b70b-d417ea4b03b4" />
<img width="782" height="672" alt="image" src="https://github.com/user-attachments/assets/c5cd2400-4baa-40ee-b0ee-c04088e01a08" />

---

# Journal 4 ( 1.5 HOURS ) :- completed the schematics 

99.9% of the schematic is complete (not 100% coz there could be smth i might have forgotten )

i did the schematic of esp32 (will use wifi and bluetooth from it) and as there is a light weight esp32 present i connected left over digital pins to it so people can use its processing power in background

<img width="1212" height="1018" alt="image" src="https://github.com/user-attachments/assets/595438b7-6103-492d-bafa-fe541c94ac02" />

i also did the wiring of pins like in an arduino uno R3 

<img width="1190" height="746" alt="image" src="https://github.com/user-attachments/assets/41f94483-31c2-4393-a45c-ec71c6abc54f" />

the extra thing is for display

completed the schematic of extra mbit flash memory 

<img width="804" height="668" alt="image" src="https://github.com/user-attachments/assets/4e9d6695-f829-4b0e-b78d-d4d1156de29e" />

also added in data lines for usb c port

oo yea i forgot i still have to select the footprints and fix erc

which uhh :( , might take some time so its only 80% complete and most time consuming and pain work starts now

<img width="1388" height="926" alt="image" src="https://github.com/user-attachments/assets/38782054-2c6e-44a5-92ac-5ef22434e36d" />
<img width="1120" height="1294" alt="image" src="https://github.com/user-attachments/assets/9db42cf6-be2c-4c2b-b926-1b3bc13cf372" />

also did the schematic of all the neo leds 

<img width="1262" height="1074" alt="image" src="https://github.com/user-attachments/assets/61759bb3-868b-455b-aca6-fa37d40c91a1" />

---

# Journal 5 ( 1 HOURS ) :- fixed all the errors and added in footprints 

fixed all the errors and added in footprints errors were mainly being pins not connected to anything and me applying wrong pwr_flag

<img width="1402" height="976" alt="image" src="https://github.com/user-attachments/assets/174de017-1713-4b3b-9c1a-6f7886e52143" />

<img width="1398" height="1136" alt="image" src="https://github.com/user-attachments/assets/74c67687-3787-4ea5-a540-7da19881c61c" />

<img width="1378" height="1136" alt="image" src="https://github.com/user-attachments/assets/47e89f11-6c05-41b0-b952-f2dc50a56412" />

---

# Journal 6 ( 1.5 HOURS ) :- started with pcb design 

first i got the laybout and size of the arduino uno r3 then i added in both planes to automatically fill up all the ground plane connections and then first placed the female headers exactly where and how they are placed in uno and then places rest of the components

resistors were pretty easy to figure out where to place because of shorter connection the better but for capacitors they were like VBUS and GND only so connections can be every hwere so i had to go back to schematic find the exact capacitor and place it as close as i can in pcb to the part it is connected to

<img width="1390" height="896" alt="image" src="https://github.com/user-attachments/assets/3f898208-84ce-40b6-9fd7-7b34351f6912" />

<img width="1260" height="918" alt="image" src="https://github.com/user-attachments/assets/3c6428c6-f870-498a-95b6-22cfdcc720f0" />

i still have a really big open area where i will prob add a bunch of art of smth like that also






