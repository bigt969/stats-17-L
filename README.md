*This is the do file for lab 3
clear // this closes any other open files
cd "C:\Stat17sect1-sp26\Lab 3"
log using lab3log.smcl, replace
use cps_in_class.dta, clear
describe // used for identifying data types
sum // summary statistics
sum pernum age 
save new_cps.dta, replace




* Now load auto.dta; use the commands for seeing the type of data or descriptive statistics of all the variables & save the data with a new file name in your favorite folder

sysuse dir

sysuse auto.dta, clear 
describe
sum
save auto78.dta, replace

log close
clear 
