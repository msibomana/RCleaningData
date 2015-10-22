# RCleaningData
Coursera Getting and Cleaning Data project

## run_analysis.R script usage
* ```data5 <- read_data5(datadir=".")``` reads training and test datasets from current(default) or user provided directory, merges the 2 datasets in a single one, computes and returns averages of each variable 
for each activity and each subject

* ```write_data5(data5, filename)``` writes data5 to filename in text format without row names

* ```read_write_data5(filename,datadir=".")``` calls write_data5(read_data5(datadir),filename)
