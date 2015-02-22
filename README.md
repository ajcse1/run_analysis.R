This script works as follows:
Step 1:Load the needed packages
Step 2:Assumes the Git repository : https://github.com/dholtz/GettingAndCleaningData
       has been cloned to a users local machine, and the R, setwd(), has been used 
       to set the working directory to the root of this cloned repository.
Step 3:Give warning to set the working directory if not able to find data files.
Step 4:Use grepl to just get features/measures related to mean and std
Step 5:Build up the columns to select from the data.table, dtSubjectActivitiesWithMeasures
Step 6:Merge the 'meaningful activity names' with the dtSubjectActiitiesWithMeasuresMeanStd
Step 7:Sort the data.table, dtSubjectActivitesWithMeasuresMeanStd
Step 8:Convert from a wide to narrow data.table using the keys created earlier
Step 9:Convert activityName and measureName to factors
Step 10:Reshape the data to get the averages
