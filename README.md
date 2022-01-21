# Adavance-SQL-operators-
Download the zip folder containing all the Advance sql operators with explaination and output 



TIME - contains only time (HOUR  , MIN , SEC )
DATE - contains only date 
TIMESTAMP - Contains date and time 
TIMESTAMPTZ - contains date,time and timezone

Careful considerations should be made when designing a table and database 
and choosing a time data type 
Depending on the situatin you may or may not need the full level of TIMESTAMPTZ 
NOTE : You can always remove historical info, but youcant add it 

Explore the FUNCTIOn and OPERATIONS related to these specific datat types:
TIMEZONE 
NOW 
TIMEOFDAY
CURRENT_TIME
CURRENT_DATE


1.shows the value of run time parameters
	SHOW ALL 

2.so one of those run time parameters you can check is 
	SHOW TIMEZONE 
(the computer you are working on current time zone will be displayed)  

3.if you wanna recall TIMESTAMPTZ : 
	SELECT NOW()  
(you ll get date and your timezone) 

4.to call timezone in STRING format 
	SELECT TIMEOFDAY()

5.gives you currenttime
	SELECT CURRENT_TIME 

6.gives you currentdate
	SELECT CURRENT_DATE

LETS EXPLORE EXTRACTING INFORMATION FROM A TIME BASED DATA TYPE USING:
1.EXTRACT()
2.AGE()
3.TO_CHAR()

1. EXTRACT()
-allows you to "extract" or obtain a sub-component of a date value 
-year 
-month 
-day 
-week
~EXTRACT(YEAR FROM date_col)

2.AGE()
-calculates and returns the current age given a timestamp 
-Useage:
~AGE(date_col)
-Returns 
~13 Years 1 mon 5 days 01:34:13.003423

3.TO_CHAR 
-General function to convert data types to text 
-Useful for timestamp formatting 
-Usage
~TO_CHAR(date_col,'mm-dd-yyyy')


