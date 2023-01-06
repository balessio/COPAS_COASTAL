Climate Data Operators (CDO) is a collection of operations for netcdf files. It is extremely fast compared to the same analysis in Python or Matlab as it does not require any memory. 

Install following these instructions:
https://www.isimip.org/protocol/preparing-simulation-files/cdo-help/

An example usage would be to type the following into your terminal:
cdo yhouravg in.nc out.nc

This computes a climatology for the data of in.nc and saves it into out.nc. Other commands and information can be found here:
https://code.mpimet.mpg.de/projects/cdo/wiki

If you have lots of commands to execute with CDO, or perhaps want to run a loop, I recommend using Bash scripting. A very basic example would be, in your terminal:
touch example.sh

then open example.sh in a text-editor, and paste the following:
cdo yhouravg in.nc out.nc

To run this command, type the following in the terminal:
bash example.sh
