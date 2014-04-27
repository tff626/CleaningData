The R codes stored in "run_analysis.R" helps to clean the UCI HAR Dataset. It takes the following steps:
1. Merges the training and the test sets to create one data set.
## Step 1. Create train table (read.csv files and cbind command);
## Step 2. Create test table (read.csv files and cbind command);
## Step 3. Combine train and test tables (rbind command);
## Step 4. Join labels.

2. Extracts only the measurements on the mean and standard deviation for each measurement. 
3. Uses descriptive activity names to name the activities in the data set.

4. Creates a second, independent tidy data set with the average of each variable.
## Step 1. split data by subjects (split command);
## Step 2. create index numbers for subject and activities;
## Step 3. calculate mean for each activity in a given subject (tapply);
## Step 4. combine subject and activity indexes with means.

5. Appropriately labels the data set with descriptive activity names.
6. Write data into a .txt file.