# Befaco_VCADSR_v1.1
Hamara Labs modified version of the Befaco version 1 VCADSR
The original files from Befaco are available here:
https://www.befaco.org/en/sinte-modular/en-produccion/vc-adsrv1/

Original design by Juergen Haible (http://www.jhaible.info/tonline_stuff/hj_vc_hadsr.html) 

and Tom Gamble (http://synthdiy.fonitronik.de/files/4613/8287/9784/vcradsr.pdf)

I fixed a couple of bugs
  1) the inputs to the unused half of the 4013 were left floating - they are now properly grounded
  2) The trigger input to the used half of the 4013 was effectively floating whenever there was no gate input present, 
  due to the reverse biased D2. Added R26 to hold the trigger input at ground when D2 is reverse biased
  3) A retrigger bug was identified by someone somewhere, and photos of a haywire patch have been routinely distributed on line.
  That mod has been incorporated on the PCB as D6 and T8
  
I also updated the layout to use parts that are more readily available than the parts used in the original design. 
  
This repository contains 2 PCBs (FRONT and BACK) and one panel, all in KiCAD (http://kicad-pcb.org/)

The BOM is at https://docs.google.com/spreadsheets/d/1yNOWsHSHRAM60BiDUVynL0L72_J8PpAY8x3tWKFwJsM/edit?usp=sharing
This file takes precedence over the BOM in the assembly instructions document.

I believe all these files are correct, but I make no warranty whatsoever. Build at your own risk. If you find any problems with these files, please contact Hamara Labs at HamaraLabs1 (at) gmail.com and I will update the files.
