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
	2. src : Has an ETL folder, with a sub-folder called Utils.
             2.1. UTILS: contains 3 files
                a. modules: with basic util functions
                b. imports: having all the required imports
                c. configs: yaml file with cofigs such as paths & columns
             2.2. BRONZE-TO-SILVER.ipynb : contains data cleaning functions and stored at SILVER layer in parquet form.
             2.3. SILVER-TO-GOLD.ipynb: contains activity specific functions as per requirement and result is stored at gold layer.
