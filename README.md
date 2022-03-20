# Thel SAC 30.2/30.3
Thel "**S**uper **A**ctive **C**rossover" (german: SA**W** 30.2/30.3) | 2-input ➔ 4-ouput | switchable: either 2-way-stereo or 3-way-mono | 24dB/Oct. Linkwitz-Riley  
realized as a 4th-order "state variable filter" according to:  
*>> Audio-Engineering-Society, Edition 1983 October 8-12, No. 2011 (B-2) by its inventor **Dennis A. Bohn**, Rane Corporation, Mountlake Terrace, Washington <<*  
➔ <a href="/docs/related/2099_AES_preprint_2011(B2)_1983.pdf">2099_AES_preprint_2011(B2)_1983.pdf</a>

maintaining a phase shift of 0° between the filter passes\* at any time at any frequency.  
*>>All in all, this results in perfect transmission in terms of time and level. The compromise is that the frequency-dependent phase rotation of this analogue filter is not shifted between the neighboring filter passes\*, but only between the input and output of the crossover.<<*  
  
\*(low-pass / band-pass / high-pass)   
<hr />

The original versions are equipped with balanced (symmetrical ) audio inputs  
but unbalanced (asymmetrical) audio outputs.
<hr />

In the <a href="/hardware">"hardware"</a> folder of this repository you can see the different versions of this module as they were built by THEL over the years and decades.  
This does NOT necessarily mean that the latest, newest version ("version 07.2017 until now") is also the "best" version.  
As you can see, in this case the sub-bass-boost feature and the extended supply voltage section is missing in the latest SAC 30.x  
and the very good PP 1% film/foil precision capacitors were switched to "normal" WIMA MKP 2.5% - 10% (or even MKS only).  
However, the latter in particular contradicts the goal of the 0° phase shift, because this requires that the determining filter capacitors and resistors have a tolerance of 1% or better (!).  
(In addition, the PP film/foil also sound better than the MKP types ➔ lower (and less frequency-dependent) dissipation factor "tan delta" etc...)  
On the other hand the latest, newest version ("version 07.2017 until now") introduces a much better input section (with 2 Op-Amps) in comparision to the previous model ("version 2011-2017")  
  
### So here is a comparison of this two versions and their specific pros and cons:  
#### Latest "version 07.2017 until now":  
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
#### Previous "version 2011-2017":  
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
### my plans:  
* in the first step I will design a new SAC30, which combines the advantages of the two versions mentioned above,  
it will still be in THT technology but 2 layer PCB, so that an average hobbyist can easily build it himself       
* the next step will be to create an all SMD version of this (eventually including 1% C0G ceramic filter caps), with some new features like symmetrical outputs, input/output EMC protection, ...)

<hr />  

## latest version as of 07.2017 until today:  
<img width="100%" src="/hardware/version 07.2017 until now/SAW302.jpg" />  
  
## better previous version (built 2011-2017):
<img width="100%" src="/hardware/version 2011-2017/SAW30-3_2011-2017.jpg" />  
  
https://web.archive.org/web/20071014012620/http://www.thel-audioworld.de/module/saw/saw.htm  
old frequency-table: https://web.archive.org/web/20160324050324/http://thel-audioworld.de/module/saw/SAWTAB.GIF  
https://web.archive.org/web/20110927050632/http://www.thel-audioworld.de/module/saw/saw.htm  
https://web.archive.org/web/20160406211449/http://www.thel-audioworld.de/MODULE/SAW/saw.htm  
https://web.archive.org/web/20180819222254/http://www.thel-audioworld.de/module/SAW/saw.htm  

----

<img width="100%" src="/docs/english (translated %26 corrected)/2-way-stereo_schema.png" />  
  
<img width="100%" src="/docs/english (translated %26 corrected)/2-way-stereo_sub-sat_schema.png" />  
  
<img width="100%" src="/docs/english (translated %26 corrected)/3-way-mono_schema.png" />  

----

here's a link to a calculation table (spreadsheet)  
to choose the right capacitors and resistors for a certain crossover frequency and to get the desired adjustment range:  
https://docs.google.com/spreadsheets/d/1a5ryznVy3UrqgniDteTX_oCJn4powWA7M3F-0194jWU/edit?usp=sharing

