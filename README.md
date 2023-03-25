# ERCF_Filament_Cutting_MOD
ERCF Filament Cutting Mod


[![Video Label]()
(https://www.youtube.com/watch?v=jHE_eaS_J6o&ab_channel=MrGoodman)

[![Video Label]()
(https://www.youtube.com/watch?v=E3OkWK-ciag&ab_channel=MrGoodman)


https://blog.naver.com/pure100kim/223006132448


**1. Using software**

I use ERCF software : https://github.com/moggieuk/ERCF-Software-V3


**2. Prepare parts**

(1) E3D V6 Heatsink  1ea
https://smartstore.naver.com/2bitmall/products/5242626620


![Image of ERCF Toolheadsensor](https://github.com/pure100kim/ERCF_Filament_Cutting_MOD/blob/main/Photos/E3DV6_HEATsink.png)



(2) Art knife  diagonal Type  1ea

https://ct5488.com/goods/goods_view.php?inflow=naverPay&goodsNo=1000144370&NaPm=ct%3Dldrdw015%7Cci%3Dcheckout%7Ctr%3Dppc%7Ctrx%3D%7Chk%3D073a0e776e0796a97f9be5310aa3d765167d25f9

![Image of ERCF Toolheadsensor](https://github.com/pure100kim/ERCF_Filament_Cutting_MOD/blob/main/Photos/ART_Knife.png)



(3) etc

-. M2*12mm 1EA

-. M2 space

-. M3*14mm 2EA

-. M3 Insert 3EA

-. ballpoint pen spring  1EA


(4) ERCF_Cutting_lever_Touch_screw holder
2020 Profile 50mm

M5 Sprint Nun or T nut 3EA

M5*30mm  1EA

M5*8mm 4EA

Corner Block 2EA






**3. STL Fils**


The (1)(2) two stl files must be combined for the blade to work properly.


(1)ERCF OMRON switch and Neodium Magectic

https://github.com/pure100kim/StealthBurner_Toolhead-Sensor_switch
![Image of ERCF Toolheadsensor](https://github.com/pure100kim/StealthBurner_Toolhead-Sensor_switch/blob/main/Picture/stealthburner_assembly.jpg)



(2) Cutting lever





**4. Assemble**

It is important teflon tube shape becase To ensure that the filament fits properly, it is necessary to shape it.

![Image of ERCF Toolheadsensor](https://github.com/pure100kim/ERCF_Filament_Cutting_MOD/blob/main/Photos/ERCF_teflon_tube_shape.jpg)


Assemble it as shown in the picture below

![Image of ERCF Toolheadsensor](https://github.com/pure100kim/ERCF_Filament_Cutting_MOD/blob/main/Photos/ERCF_Cutting_lever_assemble.jpg)






![Image of ERCF Toolheadsensor](https://github.com/pure100kim/ERCF_Filament_Cutting_MOD/blob/main/Photos/ERCF_Cutting_lever_Touch_screw%20holder.jpg)






**5. gcode macro**

Include Filament cutting macro file in printer.cfg  as below

![Image of ERCF Toolheadsensor](https://github.com/pure100kim/ERCF_Filament_Cutting_MOD/blob/main/Photos/ERCF_Filament_cutting_macro.png)


If you want move _PARK location or wiper location, change the gcode end line.


(Optinonal) Filament wiper 
https://github.com/pure100kim/VORON_NOZZLE_WIPER/blob/main/README.md





**6. Prusa Slicer setting**

![Image of ERCF Toolheadsensor](https://github.com/pure100kim/ERCF_Filament_Cutting_MOD/blob/main/Photos/ERCF_Prusa_slicer_command.png)




**7. Filament remove modification**

Modify [gcode_macro REMOVE_FILAMENT] macro section in printer.cfg

Adjust retraction lenth value This is cutting position. 

M117 Removing filament
ERCF_FORM_TIP_STANDALONE USE_SKINNYDIP=1 SKINNYDIP_DISTANCE=31 COOLING_TUBE_LENGTH=10 COOLING_TUBE_RETRACTION=35
G91
G92 E0
G1 E-35 F3000




    








