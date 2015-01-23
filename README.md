# Getting-and-Cleaning-data
##This file describes how run_analysis.R script works.
*	First, unzip the data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip and rename the folder with "data".
*	Make sure the folder "data" and the run_analysis.R script are both in the current working directory.
*	Second, use source ("run_analysis.R") command in RStudio.
*	This script makes combined data sets for the X var, the Y var and the Subject data.
*	Once these have been combined it goes into the new data and computes and extracts the mean and standard deviation of the data for each of the subject, x, and y data.
*	It then finds unique subjects, counts them, numbers the activities and runs two for loops to populate the data.
*	Third, you will find two output files are generated in the current working directory:
  *	merged_data.txt (7.9 Mb): it contains a data frame called cleanedData with 10299*68 dimension.
  *	data_with_avg.txt (220 Kb): it contains a data frame called result with 180*68 dimension.
*	Finally, use data <- read.table("data_with_avg.txt") command in RStudio to read the file. 

