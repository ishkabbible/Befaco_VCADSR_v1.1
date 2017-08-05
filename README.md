# Befaco_VCADSR_v1.1
Hamara Labs modified version of the Befaco version 1 VCADSR
The original files from Befaco are available here:
https://www.befaco.org/en/sinte-modular/en-produccion/vc-adsrv1/

I fixed a couple of bugs
  1) the inputs to the unused half of the 4013 were left floating - they are now properly grounded
  2) The trigger input to the used half of the 4013 was effectively floating whenever there was no gate input present, 
  due to the reverse biased D2. Added R26 to hold the trigger input at ground when D2 is reverse biased
  3) A retrigger bug was identified by someone somewhere, and photos of a haywire patch have been routinely distributed on line.
  That mod has been incorporated on the PCB as D6 and T8
  
I also updated the layout to use parts that are more readily available than the parts used in the original design. 
  
This repository contains 2 PCBS (FRONT and BACK) and one panel, all in KiCAD (http://kicad-pcb.org/)

If you find any problems with these files, please contact Hamara Labs at ishkabbible (at) gmail.com
