# ERCF_Filament_Cutting_MOD
ERCF Filament Cutting Mod

I use ERCF software : https://github.com/moggieuk/ERCF-Software-V3

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



