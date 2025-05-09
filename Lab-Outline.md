# HydroLight Lab

## 1. New Case 1 IOPs

### a. HydroLight

Step through the GUI for the New Case 1 IOPs model and run HydroLight

### b. EcoLight

Do the same run as before but run EcoLight

What is the difference in Rrs? What was faster? Why?


## 2. User specified IOPs

Useful for calculating the light field for modeled IOP data or IOPs measured in situ

### a. With the GUI

Step through the MEASURED IOPs options and run EcoLight

### b. Without the GUI

Use Python to build the input file (Iroot), and run EcoLight (from the command line
and/or the executable)

## 3. Submit LOTS of runs aka "batch run"

One of the real benefits of HE is being able to build a synthetic dataset. 
Imagine you had a bio-optical model where your constituents were CHL and CDOM,
and you wanted to generate Rrs spectra for a range of CHL and CDOM values.
You could step through the GUI manually entering everything, then run HE. 
This could take a long time depending on how many different combinations of CHL
and CDOM you have. 
OR you could use e.g., Python, to create all your input files, and then run all 
your input files at once.

- Use Python to build the appropriate input files and (Iroot, bbroot, and acroot)
and run EcoLight (`Create-HE-inputs.ipynb`)
- Use Python to read output from the printout files (this step is maybe redundant
with the newer version of HE that I think has a better Excel output) (`Read-HE-outputs.ipynb`)
- Plot (check with Patrick what he had in mind)