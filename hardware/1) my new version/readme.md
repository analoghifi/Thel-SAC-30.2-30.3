### Summary:  
In the <a href="/hardware">"hardware"</a> folder of this repository you can see the different versions of this module as they were built by THEL over the years and decades.  
This does NOT necessarily mean that the latest, newest version ("version 07.2017 until now") is also the "best" version.  
As you can see, in this case the sub-bass-boost feature and the extended supply voltage section is missing in the latest SAC 30.x  
and the very good PP 1% film/foil precision capacitors were switched to "normal" WIMA MKP 2.5% - 10% (or even MKS only).  
However, the latter in particular contradicts the goal of the 0° phase shift, because this requires that the determining filter capacitors and resistors have a tolerance of 1% or better (!).  
(In addition, the PP film/foil also sound better than the MKP types ➔ lower (and less frequency-dependent) dissipation factor "tan delta" etc...)  
On the other hand the latest, newest version ("version 07.2017 until now") introduces a much better input section (with 2 Op-Amps) in comparision to the previous model ("version 2011-2017")  

### Plans for \"my new version\":  
* in the first step I will design a new SAC30, which combines the advantages of the two versions mentioned below,  
it will still be in THT technology but 2 layer PCB, so that an average hobbyist can easily build it him/herself       
* the next step will be to create an all SMD version of this (eventually including 1% C0G ceramic filter caps), with some new features like symmetrical outputs, input/output ESD protection, ...)  
  
<hr>  
  
### So here is a comparison of this two versions and their specific pros and cons:  
#### Latest "<a href="/hardware/2)%20version%2007.2017%20until%20now">version 07.2017 until now</a>":  
:x: no "bass-boost" feature  
:x: using only "normal" capacitors in the filter section WIMA MKP 2.5% - 10% (or even worse: WIMA MKS)  
:x: no "Multi-Footprint" for the 8 filter capacitors (to optionally use different sizes and shapes of filter caps)  
:x: therefore no possibility to use the beloved tower style 1% precision KP film/foil caps in the filter section  
:x: no input caps in the power supply section  
:x: using of SOT-32 power transistors "only" in the power supply section (BD139/BD140 80V/1,5A/1,25W)  
:x: limited power supply voltage range of ±9V ... ±36V DC "only"  
:x: no possibility and space on the PCB to use optional (front panel mount) level potentiometers  
:x: no (RF-) bypass caps directly on the supply pins of the OP amps, although they are mandatory in every data sheet (for very good reasons)  
:heavy_check_mark: better audio input section with 2 OP-Amps (better symmetry / higher CMRR)   
:heavy_check_mark: using lower resistors in the filter section (less noise in theory)  
:heavy_check_mark: smaller dimensions (85 x 121mm)   
#### Previous "<a href="/hardware/3)%20version%202011-2017">version 2011-2017</a>":  
:heavy_check_mark: "bass-boost" feature  
:heavy_check_mark: using the high grade tower style 1% precision KP film/foil caps in the filter section  
:heavy_check_mark: "Multi-Footprint" for the 8 Filter capacitors to optionally use different sizes and shapes of filter caps  
:heavy_check_mark: 2 input caps (100µF) in the power supply section  
:heavy_check_mark: using of TO-220 power transistors in the power supply section (TIP132/TIP137 100V/8A/2,0W)  
:heavy_check_mark: extended power supply voltage range of ±9V ... ±60V DC  
:heavy_check_mark: preparation for using optional (front panel mount) level potentiometers directly on the PCB (in this case: TKD CP601 \[Conductive Plastic\])   
:x: no (RF-) bypass caps directly on the supply pins of the OP amps, although they are mandatory in every data sheet (for very good reasons)  
:x: using a simplified audio input section with 1 OP-Amp only (worse symmetry / lower CMRR)  
:x: using higher resistors in the filter section (more noise in theory)    
:x: larger dimensions (95 x 142mm)  

