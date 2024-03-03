Requirement:
Application should perform below analysis and store the results for each analysis.
1.	Analytics 1: Find the number of crashes (accidents) in which number of males killed are greater than 2?
2.	Analysis 2: How many two wheelers are booked for crashes? 
3.	Analysis 3: Determine the Top 5 Vehicle Makes of the cars present in the crashes in which driver died and Airbags did not deploy.
4.	Analysis 4: Determine number of Vehicles with driver having valid licences involved in hit and run? 
5.	Analysis 5: Which state has highest number of accidents in which females are not involved? 
6.	Analysis 6: Which are the Top 3rd to 5th VEH_MAKE_IDs that contribute to a largest number of injuries including death
7.	Analysis 7: For all the body styles involved in crashes, mention the top ethnic user group of each unique body style  
8.	Analysis 8: Among the crashed cars, what are the Top 5 Zip Codes with highest number crashes with alcohols as the contributing factor to a crash (Use Driver Zip Code)
9.	Analysis 9: Count of Distinct Crash IDs where No Damaged Property was observed and Damage Level (VEH_DMAG_SCL~) is above 4 and car avails Insurance
10.	Analysis 10: Determine the Top 5 Vehicle Makes where drivers are charged with speeding related offences, has licensed Drivers, used top 10 used vehicle colours and has car licensed with the Top 25 states with highest number of offences (to be deduced from the data)


This is a mini project done on vehicle crash data of the US. This was implemented in Jupyter notebook and uploaded.
This project has two folders:
  1. data
  2. src
-------------------------------------------------------------------------------------------------------------------
	1. data: has 3 sub-folders (BRONZE, SILVER & GOLD). 
 			 The data goes through an ETL process following a medallian architecture to get the required outcome.
 			 1.1. BRONZE: has the raw data given	
			 1.2. SILVER: is the pre-processed data, with some data cleaning functions in place
        	 1.3. GOLD: application required data results.
	2. src : Two notebooks, ETL & main, and a sub-folder called Utils.
             2.1. UTILS: contains 3 files
                a. modules: with basic util functions
                b. imports: having all the required imports
                c. configs: yaml file with cofigs such as paths & columns
             2.2. ETL.ipynb : Two classes ToSilver (data cleaning & preprocessing). ToGold: Requirement specific functions.
             2.3. main.ipynb
