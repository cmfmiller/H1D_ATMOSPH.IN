# H1D_ATMOSPH.IN

This is example Python code to automatiate editing ATMOSPH.IN files for an batch run of the HYDRUS 1D model. 

HYDRUS 1D is a numerical water and solute transport model in "variably staturated porus media" written and maintained by Jirka Simunek's group at University of California Riverside. The model is often used to model the movement of water, nutrients, and pollutants through soil profiles. To answer many questions, researchers must run the model many times with varing inputs. This script can be used as an example and/or starter code for those wishing to automate the process of creating new run files and editing ATMOSH.IN files for a batch model run. 

In this particular case my co researchers and I were running H1D many times with the same soil profile and initial conditions but slightly changed the water and solute imputs in each day. The water and solute inputs for each run were each saved in a sheet of an excel spread sheet, and loaded into the notebook as pandas dataframe. The function also requires a base path to the orignial directory containing all the hydrus input files are located. The script copys all files from the original directory into a new directory, replaces the orginal ATMOSPH.IN file with new inputs from given the excel sheet. The original directory will be copied in the same base path location, with an associated executable file. The name of the copied will be the same as the original directory with the copy number appended.

Good Luck!
