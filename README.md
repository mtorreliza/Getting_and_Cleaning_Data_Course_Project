# Getting and Cleaning Data Course Project

This project is in compliance with the requirement in completing Getting and Cleaning Data Course

This repo contains 2 files namely: run_analysis.R and CodeBook.md

===============================================================================================  

## run_analysis.R (R Script)

This explains the R script step by step.

1. Download Zip File
  * Use download.file function to download file from the url provided
  * Unzip the file using unzip function with method "wb" for zip files

2. Read Data files
  * Read txt files using read.table

3. Merges the training and the test sets to create one data set
  * Merge observations, subjects and activity data respectively
  * Renames subject and activity names

4. Extracts only the measurements on the mean and standard deviation for each measurement  
  * Use grep to extract mean() and std() characters to variable names from features table  
  * Filter merged observation table containing the list of variables filtered.  
  * Merge filtered observation data, subject and activity data.
  
5. Uses descriptive activity names to name the activities in the data set  
  * Use factor function to change the type of subject column and change its levels into descriptive names
  
6. From the data set in step 4, creates a second, independent tidy data set with the average of each  
variable for each activity and each subject  
  * Use library(reshape2) to melt column variable names into columns.
  * Use dcast to get the mean/average by subject, activity and variable name.
  * Melt the data again to create the final tidy data set
  
## CodeBook.md

Explains all the tables and datasets used

