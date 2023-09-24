this is not the original Thel PCB but it's very like\* the original with the following exceptions:  
* more massive ground and power supply PCB tracks  
* using the 2mm gold-plated brass solder pins (the same ones used on the more expensive Thel modules)
* using a combined 5.0mm/7.5mm pin spacing footprint for all of the foil caps (C1 - C8, C13,C14) 
  
\*(same schematic / same board dimensions / same 1-layer\*\* layout THT / same THT components in the same places on the board)  
\*\*(strictly speaking, this KiCad PCB is a two-layer PCB with plated-through holes, but you can also (let) produce it as a classic 1-layer PCB with non-plated holes if you wish, since all the tracks are on the bottom side only)  
  
----  
  
### remarks:  
#### U1,U2,U3,U4:  
instead of [MC33079](https://github.com/analoghifi/Thel-SAC-30.2-30.3/blob/main/docs/components%20datasheets/MC33079_Motorola.pdf) you can use
2 pieces\*\* of the dual op amp [LME49720](https://github.com/analoghifi/Thel-SAC-30.2-30.3/blob/main/docs/components%20datasheets/LME49720.pdf) or [LM4562](https://github.com/analoghifi/Thel-SAC-30.2-30.3/blob/main/docs/components%20datasheets/LM4562.pdf) (both\* Texas Instruments),  
with slightly better technical data regarding noise an THD.  
  
\*(these two are 100% identical (even regarding their inner guts))  
  
\*\*(two pieces of dual op amps replace one of the quad op amp MC33079 - you have to use an adapter-PCB for it  
-> search for "dual-opamp to quad-op-amp adapter" on google -> there are different versions available.  
The adapter (target) footprint has to be 14-pin DIP with pins on a 0.1 inch pitch in rows spaced at 0.3 inch)
  
----  
  
these are KiCad 6.x projects  
see how to get the proper 3D-Models from here: https://github.com/analoghifi/KiCad-3D-Models


