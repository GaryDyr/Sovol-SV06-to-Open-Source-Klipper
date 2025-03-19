The file, sv06_to_klipper.pdf, is a running tutorial history of changing a stock Sovol SV06 printer from Marlin to open source Klipper. It describes the process, trial and trbulations of the changeover, and calibrations needed.

The file,  klipper_bed_leveling_experiments.pdf, lays out the problems of trying to achieve a level bed with the standard inductive probe of the SV06. It deals with issues where the inductive probe cannot faithfully resolve the bed surface. Potential reasons for the lack of correlation are discussed. 
The Bed_Calc.xlsm file is an Excel file that is associated with the bed leveling experiments. It contains calculation methods related to adjusting the Z tilt, and how the klipper bed mesh calibration data was manually altered to achieve good first layer prints.

The 3x3 first layer print used for first layer uniformity is included. 

A new calibration "tree" model files that are used to calibrate the x and y stepper motor settings is also included. 

A copy of the final printer.cfg file that was used for this effort is included. For new Klipper users, be forewarned that a number of parameters in this file are highly printer specific and unlikely to be the same for you printer, even if an SVO6. For example: most, if not all of the SAVED_CONFIG section, is not likely to work. Any parameters that are dreived by calibration should be viewed with skepticism. It is encouraged to just download the basic Klipper github SV06 file as a starting point, and compare differences with the printer.cfg file here. Read over the sv06_to_klipper.pdf sections on various calibrations, before making changes to the printer.cfg file; this will help you understand what might be usable. 
