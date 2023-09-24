this is not the original Thel PCB but it's very like\* the original with the following exceptions:  
* more massive ground and power supply PCB tracks  
* using the 2mm gold-plated brass solder pins (the same ones used on the more expensive Thel modules)
* make use of my \"universal capacitor footprint\" for the filter caps (C1 - C8) -> see here T.B.D.
* using a combined 5.0mm/7.5mm pin spacing footprint for the two bypass (foil) caps (C17, C18) 
  
\*(same schematic / same board dimensions / same 1-layer\*\* layout THT / same THT components in the same places on the board)  
\*\*(strictly speaking, this KiCad PCB is a two-layer PCB with plated-through holes, but you can also (let) produce it as a classic 1-layer PCB with non-plated holes if you wish, since all the tracks are on the bottom side only)  
  
----  
  
### remarks:  
#### U1,U2,U3,U4:  
instead of [MC33079](https://github.com/analoghifi/Thel-SAC-30.2-30.3/blob/main/docs/components%20datasheets/MC33079.pdf) you can use [OPA1604](https://github.com/analoghifi/Thel-SAC-30.2-30.3/blob/main/docs/components%20datasheets/OPA1604.pdf),  
with slightly better technical data regarding noise an THD.
  
----  
  
these are KiCad 6.x projects  
see how to get the proper 3D-Models from here: https://github.com/analoghifi/KiCad-3D-Models


