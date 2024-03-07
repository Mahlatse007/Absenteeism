# Absenteeism
Preprocessing data using Pandas library.


This script aims to preprocess absenteeism data stored in a CSV file named "Absenteeism-data.csv" using the Pandas library. It performs various data cleaning and manipulation tasks to prepare the data for further analysis. The preprocessing steps include dropping unnecessary columns, encoding categorical variables, extracting features from the date column, and reordering columns.


1. Importing the Packages:
   - This section imports necessary packages, such as Pandas.

2. Importing the Data:
   - Reads the absenteeism data from the CSV file into a Pandas DataFrame.

3. Making a Copy of the Data:
   - Creates a copy of the original DataFrame to preserve the integrity of the original data.

4. Dropping 'ID' Column:
   - Removes the 'ID' column from the DataFrame as it's not needed for analysis.

5. Encoding 'Reason for Absence' Column:
   - Encodes the 'Reason for Absence' column using one-hot encoding.

6. Grouping the Reasons for Absence:
   - Groups the encoded 'Reason for Absence' columns into four types based on predefined ranges.

7. Concatenating Column Values:
   - Concatenates the grouped 'Reason for Absence' columns with the original DataFrame.

8. Reordering Columns:
   - Reorders the columns for better readability and analysis.

9. Converting 'Date' Column:
   - Converts the 'Date' column to datetime format.

10. Extracting Month and Day of the Week:
    - Extract the month and day of the week from the 'Date' column.

11. Mapping 'Education' Column:
    - Maps the 'Education' column values to binary values for simplification.

12. Creating Checkpoints:
    - Creates checkpoints at various stages to preserve intermediate results.

13. Final Checkpoint:
    - Saves the preprocessed DataFrame as the final cleaned dataset.
