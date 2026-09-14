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

---

# Journal 7 ( 1.3 HOURS ) :- gpio pins done of female headers 

firstly i made 2 more planes one for gnd and one for power management and i also added in net classes and increased constraints so there will be no problem eben if it is made offline then i did the routing of gpio pins of female headers and i also plan it to submit to kicad competition so i am trying to make as clean of routing as possible (also the reason why i increased some constraints )

<img width="758" height="982" alt="image" src="https://github.com/user-attachments/assets/d8b83f79-e2f1-4dd0-a376-71305171b011" />

<img width="1402" height="740" alt="image" src="https://github.com/user-attachments/assets/de224b0b-a922-46bd-9eac-141de68411fa" />

<img width="1352" height="874" alt="image" src="https://github.com/user-attachments/assets/ce46f604-3d78-4bfc-8b33-0da9f212be11" />

<img width="1332" height="1034" alt="image" src="https://github.com/user-attachments/assets/cbc1c45d-67c2-4068-be41-1c5a1c66d4ba" />

<img width="1310" height="944" alt="image" src="https://github.com/user-attachments/assets/f6baeab6-8807-4075-a9fd-e32b188f6cfe" />

---

# Journal 8 ( 2 HOURS ) :- routing almost completed 

first thing 1st i made 2nd plane as vcc so it made routing a little easier and added patches of vbus in it to make vbus also a little easier (i also passed the data lines through it to make it a little more easier as they needed to be length matched which i also did )

the length match is so perfect the difference between the length of power lines is 0.08mm

i also did routing of other components

<img width="1372" height="970" alt="image" src="https://github.com/user-attachments/assets/ecfbd210-730a-432e-8649-c5bb26988d12" />

<img width="1350" height="938" alt="image" src="https://github.com/user-attachments/assets/b193f829-0dd1-425c-a7ea-af083c5a98ac" />

i initially though of writing it journal once the whole routing process is complete but i did now because i just realised that the arrangement of neo leds is wrong and i can really route them easily i will have to use 2 planes and i think i would preffer to delete the current routing and rearrange them

---

# Journal 9 ( 1 HOURS ) :- fixed the neo pixel led routing 

<img width="1376" height="614" alt="image" src="https://github.com/user-attachments/assets/991b1a72-2024-41f3-a088-0c10dd2e7d39" />

fixed the neo pixel leds and a little more routes here and there

the neo pixel arrangement and routing looks so good i love it 

<img width="1384" height="1074" alt="image" src="https://github.com/user-attachments/assets/3bc8c418-9bb3-4007-b02d-16fc93bf3706" />

adding it extra time to avoid a huge mess and make the routing look cool was so worth it

---

# Journal 10 ( 0.5 HOURS ) :- completed the routing 

firstly i completed all the routing that was left (except 3 that are interconnecting i will have to switch from schematic kinda making a x with triple line )

and removed all the text of value and number of capacitor and resistor and all the components so it will look a little bit better

<img width="1388" height="838" alt="image" src="https://github.com/user-attachments/assets/80258dad-f000-41e3-bb31-a5cd95ec30fb" />

i also ran drc check and emm ahh what do i say 

<img width="1242" height="972" alt="image" src="https://github.com/user-attachments/assets/3451f581-d098-43d8-8354-e08987dc437d" />

it will prob take me a while

---

# Journal 11 ( 2 HOURS ) :- fixed all the errors and a bit of designing 

first i had to deal with errors some were caused because of text on routing some were because of missed routing or traces i accidently deleated or some were because of clearance being too big which was my bad and some were because planes werent connected like gnd and 5v ( i mean small patches on that plane that werent connected to the main patch )

i selected each one did hit and trial and somehow stuff worked out

i also spent time learning and designing the board to make it look cool i wanted to add hack club dino svg but i couldnt find it

i will ask on slack if i could find and submit with that in final design

also 3 warnings that are left are of no issues

<img width="1048" height="766" alt="image" src="https://github.com/user-attachments/assets/6bc8bdc9-7012-4c95-90a3-02be0335b9c9" />

<img width="1350" height="1078" alt="image" src="https://github.com/user-attachments/assets/f49068b4-69ad-4d3b-a474-fa84a0a08694" />

<img width="1324" height="1032" alt="image" src="https://github.com/user-attachments/assets/a9ce674c-96a6-4853-91bc-46222c26d46a" />

---

# Journal 12 ( 2.5 HOURS ) :- finalization 

while i was getting 3d render of the board i realised the usb c port was in the wrong direction so i had to go back to the pcb design rotate the usb c 180 degree and do all the routing of it again ( i switched tags of + data line and - data line in schematic because it was making a x so it was making it much harder to route. i also length matched them again) then i fixed all the erc errors because of left out routes and that small patch thing not connected to big patch

then i did some changes in the design by changing location of the rp - 2040 thoese lines and 3 and adding in dino

then i decided to import 3d model of the parts that werent visible in the 3d viewer i got them online imported them and for some reason importing the 3d model once for neo led wouldnt make it so that all of them automatically import that 3d model, so i had to manually select each one and upload the 3d model to it

then i decided to change the colour of the pcb to black because it looks better in my opinion and then i took some render images of it

then i made a banner for it that i applied above ( this one took me a while because i didt knew the scale of the banner and i wanted it to be perfect so i just did some hit and trial until it worked)

and final thing last i made the github repo of then entire project

<img width="1152" height="684" alt="image" src="https://github.com/user-attachments/assets/494abed3-81fa-4897-9a4e-6739f5b01695" />

<img width="1102" height="770" alt="image" src="https://github.com/user-attachments/assets/656f46cc-d4c4-4efe-ad89-440d5f4bbda7" />

---

# Journal 13 ( 2 HOURS ) :- selected components and found more problems 

i started by selecting main components rp2040 , esp 32 wroom2 , W25Q128JVS , AP2112K-3.3 , WS2812B-2020 then i noticed that the led needs 5v to run which i have already given it but the input was coming from rp2040 which is 3.3v so i had to add 74AHCT125 and select component for that too and i checked all the pins , footprint and read their datasheets to find if i had any thing that i missed and i also updated the github BOM but then while routing 74AHCT125 i noticed all the traces are of equal length then i noticed that in board setup up i did setup the net classes but i named them 3v3 and 5v instead of VBUS and VCC also i wrote YSB_DN and its pretty embarrassing ngl

<img width="1388" height="680" alt="image" src="https://github.com/user-attachments/assets/8ffeeb4d-12a9-44f4-a2aa-927b831171cf" />

so i tweaked the setup a bit fixed it and when i applied them umm i got 187 errors 

<img width="1188" height="1064" alt="image" src="https://github.com/user-attachments/assets/fe42daab-65fa-4476-b339-650272a34211" />

<img width="1222" height="476" alt="image" src="https://github.com/user-attachments/assets/410a0549-9b8a-4bdb-98b3-c1acd2077fc0" />

---

# Journal 13 ( 5.2 HOURS ) :- fixing mistakes 

i went through every single error and warning earlier there were

<img width="1182" height="1272" alt="image" src="https://github.com/user-attachments/assets/2e3cd379-f3cc-441c-a827-191a1ac030c2" />

problems like this all over the board i had to add a lot of trace width 

<img width="878" height="1166" alt="image" src="https://github.com/user-attachments/assets/de3bcb67-135c-4de2-ade8-f7328cb54d30" />

and then when i was fixing i used the new trace width and whenever i encountered a point where i couldn't use the default ones i set i went from the top to bottom of these ones i added until i found the one which perfectly fits trying to making them as thick and possible and as short as possible at the same time to make them short i used the trick called fan out where i made a short trace (i tried to make it shorter then 50mils) which then connects to a thicker trace or a via

also i had to again length match the usb c data lines again and they only have a difference of 4 mils now

and here is what final pcb looks like 

<img width="1282" height="924" alt="image" src="https://github.com/user-attachments/assets/a958542b-0c0f-4835-8f45-bb7ebcaf8dc8" />

<img width="1212" height="1160" alt="image" src="https://github.com/user-attachments/assets/600fde5d-4dd3-47ac-8f44-a998f3b705a1" />

<img width="1320" height="1094" alt="image" src="https://github.com/user-attachments/assets/3645e3da-6b7d-4c37-9141-e3640ee83496" />

this part took me 3.2 hr

the more i am reading my journals the more mistakes i am finding 

<img width="1292" height="634" alt="image" src="https://github.com/user-attachments/assets/2aa84ad6-9afc-44a4-8fc1-57b85fe68ff9" />

why did i use resistor footprints for capacitor i prob just went with the flow and spam clicked the button

<img width="778" height="476" alt="image" src="https://github.com/user-attachments/assets/9bc9518d-3f3a-4551-9e5e-d050efdc07d9" />

why did i legit thought they go in opposite direction like + with - and - with +

i think i should get a rubber ducky to explain everything i did

ig i wasnt reading datasheets that often or not with much attention

<img width="1388" height="1016" alt="image" src="https://github.com/user-attachments/assets/7610d765-b091-4d86-b463-b6dd1e926a8f" />

<img width="1338" height="1222" alt="image" src="https://github.com/user-attachments/assets/7fe22d5c-d52f-4cbf-a1cf-0218447bf4cb" />

<img width="1364" height="1264" alt="image" src="https://github.com/user-attachments/assets/4a6d4168-8692-4264-9c4d-cd544494d178" />

also i length matched them they both are 1742 mils now 

<img width="1404" height="1272" alt="image" src="https://github.com/user-attachments/assets/cd7cb2e4-7051-4e94-b4bd-cd0a3f3e0ebf" />

i also got hit by 5 errors and 9 warning i also went around the whole pcb remove all the small text things i forgot what they were called like u5 etc and values of capacitor i removed all of them and fixed all the issues with the pcb"

and finally i selected all the components (the buttons are lowkey expensive like way expensive then i thought i tried finding an alternative but these ones are the perfect match)

this part took me 2 hrs

i accidentally missed a journal while transferring so i had to merge these together

---

# Journal 14 ( 1 HOURS ) :- pretty much complete 

i tried finding a crystal ossicator that will work with rp2040 based on my current footprint and i found an high quality one but it has load capacitance of 8 pF so i was to switch the capacitors to 10pF (if i am wrong then correct me the formula is c = 2 x (load capacitance - stray capacitance) so c = 2 x (8 - 3) , c = 10 ) 

<img width="1368" height="886" alt="image" src="https://github.com/user-attachments/assets/7c84dbd8-c8d0-42d2-afed-dab25bc21aed" />

so yea it was a quick fix for it no need to change anything in schematic or footprint i did check the datasheet and its pretty vague it does tell about 2 and 4 being gnd but not about other pins but usually all 4 pin ones have the same pins so ill take a gamble with this one

---

# Journal 15 ( 0.5 HOURS ) :- final list 

i am making final adjustments and changes before submitting for grant 

<img width="1388" height="556" alt="image" src="https://github.com/user-attachments/assets/c9777b0d-e6c5-49bf-816d-a7da0147dc95" />

ROBU CART 

<img width="1070" height="1248" alt="image" src="https://github.com/user-attachments/assets/b016a1ca-ea12-456d-9851-a57cb433a0ff" />

<img width="1064" height="1200" alt="image" src="https://github.com/user-attachments/assets/b6c69a02-55d9-48ec-aa4a-74cc76aa79d3" />

<img width="1034" height="1154" alt="image" src="https://github.com/user-attachments/assets/3008c6b2-db92-4e62-a795-a19ad7e5195e" />

Evelta cart 

<img width="1074" height="812" alt="image" src="https://github.com/user-attachments/assets/23259dea-0a67-403e-9c71-57436b0028f4" />

<img width="874" height="1308" alt="image" src="https://github.com/user-attachments/assets/87a9371f-c348-4ba2-a7c1-9754e0faaa88" />

<img width="906" height="1298" alt="image" src="https://github.com/user-attachments/assets/333a7e48-03d2-4a27-aefe-56c9497b65b5" />

lion circuit cart 

<img width="1074" height="616" alt="image" src="https://github.com/user-attachments/assets/114abb1c-7db2-4c7b-9823-d511e72fbebc" />

<img width="768" height="850" alt="image" src="https://github.com/user-attachments/assets/14823913-cbed-4ae5-83e1-b7d08fed0a14" />

robu pcb 

<img width="1072" height="566" alt="image" src="https://github.com/user-attachments/assets/69b3564d-86c6-4b72-9670-638f278782df" />

<img width="1028" height="1152" alt="image" src="https://github.com/user-attachments/assets/0101fc35-b00c-4e64-8ea6-e4a889f3c7b7" />

<img width="1963" height="757" alt="image" src="https://github.com/user-attachments/assets/83289c87-e499-4047-a248-7f46076bef9b" />

<img width="507" height="1016" alt="image" src="https://github.com/user-attachments/assets/b08dc38e-186a-4a22-b749-c4a4c33ed16d" />

---

# Journal 16 ( 0.5 HOURS ) :- fixing all the errors

(my project got reviewed on forge and this is what they said :- You are missing all of your decoupling capacitors. There may be a brownout during operation. Also, i noticed that you name the values of your passives as "__1 __2 ..." Please don't do that because kicad will treat them as separate components, which is not the best practice. For future projects, please follow general conventions for your schematic since it is very hard to read.)


thanks for such a great overview a lot of things went over my head and i messed up some things so i am really thankful that you told me every reason my board would have failed it advanced i will also be going through the datasheets of chips etc to see if i missed anything else

so imma first start with fixing all the resistors and capacitor and led names 

<img width="1210" height="458" alt="image" src="https://github.com/user-attachments/assets/7f55d55a-f679-4eb6-9ffb-37b5bcf1e70f" />

<img width="1360" height="1142" alt="image" src="https://github.com/user-attachments/assets/ca19200c-5500-4f71-b829-622080f46bf7" />

changed these to this 

<img width="658" height="664" alt="image" src="https://github.com/user-attachments/assets/296dac9c-397f-4e4d-991e-1e0a09ff11e4" />

i am also verifying that capacitors are near the component they are placed for or not 

<img width="1092" height="1082" alt="image" src="https://github.com/user-attachments/assets/b54e5e95-a835-46eb-bd03-71554c73fc97" />

and i noticed there is a lot of gap in some capacitors c4 is close but c3 and c5 are really far 

<img width="1156" height="910" alt="image" src="https://github.com/user-attachments/assets/b5c9a306-abca-417f-9cff-36659af919fb" />

and i need to have more resistors and capacitors for usb and rp2040 chip i am also reading and re checking everything in hardware design 2040 pdf i will have to add 

<img width="684" height="284" alt="image" src="https://github.com/user-attachments/assets/8e0485a1-5c4f-459b-9a64-87ea8647cc6f" />

in next journal

---

# Journal 17 ( 5.5 HOURS ) :- fixing and rechecking everything

i am point point by point of hardware designn of rp2040 and checking and fixing everything first was input supply which was already correct 

<img width="650" height="636" alt="image" src="https://github.com/user-attachments/assets/6ec29839-b75e-4912-94e0-d4775b78bb3f" />

second was Decoupling capacitors so i added as much as the guide said 3 are connected directly and 4 will be placed close to those 3 this should help in having less interference 

<img width="1258" height="856" alt="image" src="https://github.com/user-attachments/assets/92c6691f-3d5e-4aa8-9891-03fc7ef66641" />

third was internal voltage regulator that is shown in above screenshot

fourth was flash storage which was fine already i just have to add a capacitor 

<img width="1044" height="974" alt="image" src="https://github.com/user-attachments/assets/3500b384-4fc7-4b3c-9cbe-a5d30e74450e" />

<img width="798" height="398" alt="image" src="https://github.com/user-attachments/assets/482c2981-c67f-44c6-9645-797e191ddee1" />

i also moved the switch a bit close in the schematic which will be used to force the RP2040 into USB mass storage mode

a bit later i realized io3 and 0 were swapped so i fixed it 

<img width="666" height="720" alt="image" src="https://github.com/user-attachments/assets/c033d0d8-990c-4fe2-9903-357da2a29378" />

fifth was crystal oscillator in this i first added the value of it and then changed the value of capacitors from 10 to 15pF and added in the resistor 

<img width="1008" height="496" alt="image" src="https://github.com/user-attachments/assets/6a496b89-4e11-4f2a-83f0-99f626047d35" />

also while making this i had to recheck it a few times because initially i made the mistake of connecting capacitor to rp2040 instead of between xout pin resistor

sixth was USB and it was correct before hand 

<img width="644" height="766" alt="image" src="https://github.com/user-attachments/assets/795ec7f0-296d-4840-97a2-a6fd71511d40" />

<img width="482" height="120" alt="image" src="https://github.com/user-attachments/assets/7a6b4b02-2823-4308-9329-de6bec4a266e" />

sevent were io pins and most of it was fine i fixed swd added in uart (earlier i had uart tags on esp 32 but on on the headers) and i also added in switches needed to put esp 32 into boot mode 

<img width="1128" height="932" alt="image" src="https://github.com/user-attachments/assets/501ae8cc-8a5f-4249-8a8f-23b397221203" />

<img width="1096" height="744" alt="image" src="https://github.com/user-attachments/assets/fbe958ae-879c-4482-81a3-e032a9e6f459" />

so now i have 3 ways to code rp2040 chip 1 usb c port 2 swd 3 uart

quick thing i checked which had an error was esp 32 c3 's boot pin is actually io9 so i moved the tag a bit

<img width="1100" height="1134" alt="image" src="https://github.com/user-attachments/assets/7fd0c788-1ec5-40a1-b13d-1f7c51b4b44c" />

i also fixed the led matrix 

<img width="1104" height="610" alt="image" src="https://github.com/user-attachments/assets/dafe079b-db7a-4ad3-afda-ddf5c81d7a9a" />

<img width="1276" height="924" alt="image" src="https://github.com/user-attachments/assets/b409f063-e0b9-4770-b57c-80da266a88ee" />

added in a big capacitor of 470μF and small capacitor for each leds

and this is where the main parts of the document ends i rechecked everything and it should work just fine

i also fixed 2 erc errors i had both were because of pins not having X tag 

<img width="1640" height="934" alt="image" src="https://github.com/user-attachments/assets/a312b221-7b7f-4661-9818-fb485a26fe36" />

<img width="1712" height="1392" alt="image" src="https://github.com/user-attachments/assets/d678b47d-e0fb-4d83-976d-7bf490def477" />

idk about the warnings ill try to find what each warning means

---
## i made a small rpp-2040 dev board in between and i learnt a bit and used footprints i have never used before and overall even though the dev board was rushed i still learnt a lot and its been a month since i made this project so i will quickly complete it now 

# Journal 18 ( 2 HOURS ) :- cleaned up the schematic 
firstly i changed the footprints to smaller ones

<img width="1202" height="1204" alt="image" src="https://github.com/user-attachments/assets/eb6f2a4c-f472-4b6e-8f4b-b2c551eaf08f" />

<img width="1774" height="862" alt="image" src="https://github.com/user-attachments/assets/19e1c6cc-6cba-4311-849f-94b18b2e387f" />

then i perfectly cleaned up the schematics 

<img width="1400" height="702" alt="image" src="https://github.com/user-attachments/assets/def467b8-eb6a-4af8-894b-1d9e0f8393cf" />

now i have to do the routing part 

<img width="978" height="614" alt="image" src="https://github.com/user-attachments/assets/3eb5aa84-c6e0-4ec8-9fbe-1bb69c0592d6" />

<img width="1050" height="688" alt="image" src="https://github.com/user-attachments/assets/06814645-2e5d-4fbb-8154-729b9a5a1cb6" />









