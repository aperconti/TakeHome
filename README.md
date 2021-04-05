## GovInvest Take Home

To process this data, I exported the excel files to CSV's and read them into Python using the Pandas library. I used Jupyter Notebook as a way to automate cleaning tasks and validate data findings efficiently. The cleaned version of this file is written to an excel file and is included in this repo. 
I spend 1.5 hours on this assignment. 

### 1)Janna K's last name changed since the previous year.  This could be true but may need to be double-checked.
There is a change to Janna's marital status between 2017- 2018, which likely accounts for the last name change.


### 2) The sex field for Andrew H. was "E", but likely should have been "M"
This field has been changed from "E" to "M"

### 3) There is an error in the birthdate of Nicholas B., which makes it seem that he is one year old.  This is a discrepancy from the prior year's data. 
This discrepancy is actually the case with JONATHAN K. Nicholas B was born in 1985 and is 32 years old. JONATHAN K, however, was born in 2016 and had an age of 1 recorded. JONATHAN K also has a hire date prior to his date of birth; this date is also in the future, which is highly suspect. JONATHAN's birthday was corrected to 5/8/1976, which was the date provided in the 1.1.2017 Data. 

### 4) There are several errors in the hire dates.  One of the new employees, Cortnie A., has a hire date of over a decade ago, Nicholas B. has a hire date in the future, and two others have varying hire dates compared to the previous year's data.
Andrew H, and DUANE T. were supposedly hired in 2015, but there is no record of them in the 1.1.2017 data set. 
Cortnie A, was supposedly hired on 8/6/07, but there is no record of her in the 1.1.2017 data set. 
NICHOLAS B. has a hire date in the future on 8/4/19

### 5) Brian T. was supposedly terminated in 2015, but there was no mention of this in the prior year.
This individual has an active status in both the 2017 and 2018 data sets. In the 2018 data set, Brian T. had a termination date of 7/1/15. Further data would be needed to verify this termination date. 

### 6) Dan H. retirement date is inconsistent with the previous data
Dan H. is the only individual with an inconsistent retirement date between the 2017 and 2018 data sets. Further data would be needed to verify this retirement date, but the date of 5/29/2009 seems to be the more reasonable of the two dates since Dan would be retiring at 36 years old with the retirement date of 3/1/1990. 

### 7) Joe H. had a change in spouse's birthdate to N/A; this could be due to several causes, but it is a potential error.
This change could be accounted for this a marital status change. Further data would be needed to verify this change. 

### Further finds: 

1)	The code cell that is calculating birthdays in the 2017 dataset is wrong. It is calculating their age by today's date, not the 1.1.2017 date that the data was pulled on. This error makes everyone older in the 2017 data set than they are in the 2018 data set. I rectified this problem by putting a date in R2 and calculating age based on this value instead of today's date. (This change was made in Excel)

2)	There are two more columns in the 2018 data set than there are in the 2017 data set. These columns are Retirement after Hire and Termination after Hire. These look like calculated fields. 

3)	The retirees that are disabled are not receiving any pensions. The years of employment for the vested employees are not consistent. This information is suspect but could be due to different vesting timelines for executives, advisors, or employees. Further data would be needed to verify this inconsistency. 



