---
output: pdf_document
---
## run_analysis.R script usage
* ```data5 <- read_data5(datadir=".")``` reads training and test datasets from current(default) or user provided directory, merges the 2 datasets in a single one, computes and returns averages of each variable 
for each activity and each subject

* ```write_data5(data5, filename)``` writes data5 to filename in text format without row names

* ```read_write_data5(filename,datadir=".")``` reads and writes data5 by calling write_data5(read_data5(datadir),filename) 

## Output data format
Column|    Variable name       | Variable description
----- |------------------------|-------------------------
1     |Subject                 | Subject ID (1-30)   
2     |Activity                | Test performed(1=WALKING, 2=WALKING_UPSTAIRS,3=WALKING_DOWNSTAIRS,4=SITTING, 5=STANDING,6=LAYING
3     |Dataset                 | Data set factor (test,train)
4-6   |tBodyAccMean[X-Z]       | Time domain Body Acceleration Mean in X,Y, Z directions
7-9   |tGravityAccMean[X-Z]    | Time domain Gravity Acceleration Mean in X,Y, Z directions
10-12 |tBodyAccJerkMean[X-Z]   | Time domain Body Acceleration Jerk Mean in X,Y, Z directions
13-15 |tBodyGyroMean[X-Z]      | Time domain Body Angular velocity Mean in X,Y, Z directions
16-18 |tBodyGyroJerkMean[X-Z]  | Time domain Body Angular velocity Jerk Mean in X,Y, Z directions
19    |tBodyAccMagMean         | Time domain Body Acceleration Magnitude Mean
20    |tGravityAccMagMean      | Time domain Body Gravity Acceleration Magnitude Mean
21    |tBodyAccJerkMagMean     | Time domain Body Acceleration Jerk Magnitude Mean
22    |tBodyGyroMagMean        | Time domain Body Angular velocity Magnitude Mean
23    |tBodyGyroJerkMagMean    | Time domain Body Angular velocity Jerk Magnitude Mean
24-26 |fBodyAccMean[X-Z]       | FFT domain Body Acceleration Mean in X,Y, and Z directions
27-29 |fBodyAccJerkMean[X-Z]   | FFT domain Body Acceleration Jerk Mean in X,Y, and Z directions
30-32 |fBodyGyroMean[X-Z]      | FFT domain Body Angular velocity Mean in X,Y, and Z directions
33    |fBodyAccMagMean         | FFT domain Body Acceleration Magnitude Mean
34    |fBodyBodyAccJerkMagMean | FFT domain Body Acceleration Jerk Magnitude Mean
35    |fBodyBodyGyroMagMean    | FFT domain Body Angular velocity Magnitude Mean
36    |fBodyBodyGyroJerkMagMean| FFT domain Body Angular velocity JerkMagnitude Mean
37-39 |tBodyAccStd[X-Z]        | Time domain Body Acceleration Stdev in X,Y,Z directions
40-42 |tGravityAccStd[X-Z]     | Time domain Gravity Acceleration Stdev in X,Y,Z directions
43-45 |tBodyAccJerkStd[X-Z]    | Time domain Body Acceleration Jerk Stdev in X,Y,Z directions
46-48 |tBodyGyroStd[X-Z]       | Time domain Body Angular velocity Stdev in X,Y,Z directions
49-51 |tBodyGyroJerkStd[X-Z]   | Time domain Body Angular velocity Jerk Stdev in X,Y,Z directions
52    |tBodyAccMagStd          | Time domain Body Acceleration Magnitude Stdev
53    |tGravityAccMagStd       | Time domain Body Gravity Acceleration Magnitude Stdev
54    |tBodyAccJerkMagStd      | Time domain Body Acceleration Jerk Magnitude Stdev
55    |tBodyGyroMagStd         | Time domain Body Angular velocity Magnitude Stdev
56    |tBodyGyroJerkMagStd     | Time domain Body Angular velocity Jerk Magnitude Stdev
57-59 |fBodyAccStd[X-Z]        | FFT domain Body Acceleration Stdev in X,Y, and Z directions
60-62 |fBodyAccJerkStd[X-Z]    | FFT domain Body Acceleration Jerk Stdev in X,Y, and Z directions
63-65 |fBodyGyroStd[X-Z]       | FFT domain Body Angular velocity Stdev in X,Y, and Z directions
66    |fBodyAccMagStd          | FFT domain Body Acceleration Magnitude Stdev
67    |fBodyBodyAccJerkMagStd  | FFT domain Body Acceleration Jerk Magnitude Stdev
68    |fBodyBodyGyroMagStd     | FFT domain Body Angular velocity Magnitude Stdev
69    |fBodyBodyGyroJerkMagStd | FFT domain Body Angular velocity JerkMagnitude Stdev

