# ERCF_Filament_Cutting_MOD
ERCF Filament Cutting Mod

1. Using software
I use ERCF software : https://github.com/moggieuk/ERCF-Software-V3


2. Prepare parts
1) E3D V6 Heatsink  1ea
https://smartstore.naver.com/2bitmall/products/5242626620



2) Art knife  diagonal Type  1ea

https://ct5488.com/goods/goods_view.php?inflow=naverPay&goodsNo=1000144370&NaPm=ct%3Dldrdw015%7Cci%3Dcheckout%7Ctr%3Dppc%7Ctrx%3D%7Chk%3D073a0e776e0796a97f9be5310aa3d765167d25f9

3) etc

M2*12 1EA
M2 space
M3*14 2EA
M3 Insert


3. STL Fils




4. Assemble



5. gcode macro

Include Filament cutting macro file in printer.cfg  as below



[gcode_macro FILAMENT_CUTTING]
#Include FILAMENT CUTTING command in Pruds slice BEFOR TOOLCHANGE gcode box
#This G1 Position is cutting rever position.Depend on Need to change position installation.
gcode:
    G92 E0
#    G1 E-40 F3000
    G1 X30 Y36 F5000
    G1 X1 Y36 F1000
    G1 X30 Y36 F5000
    G1 E-35 F3000
    G1 X20 Y300 F5000
