Doc for calculations


For each data line, the program check the max number of confirmed. If below 20 - nothing is added.
If 20 or more, the following attributes are added:

5% date - the first date where the number of confirmed is at least 5% of the max number
last relevant date- the list of 'confirmed' for each date is considered until the growth rate is 
	below 2% and remain below 2% untill the last date on file. In case where the last date is 2% or above, the 
	last date equal the last relevant date. 
GFQ1. GFQ2 . GFQ3.  THe list of growth rates , between the 5% date and the last relevant date, 1st median and 3rd 
                    quartile. Note that a 0 in the 1st quartile is valid as there are dates with no growth often.
first_7  . In cases where after the 5% date, there are 7 more dates in the file, this is the growth rate from the 
           5% date to 7 days after. It is for the entire 7 days, 1 means that the amount of confirmed was doubled

The list of growth rates (ratios)- for the first positive 'confirmed' the growth rate is set to 0. 
The gr is also 0 for any consequtive equal 'confirmed' . So 0 in the GFQ1 is valid ,esp. for locations with small 
number of total confirmed.




 
   