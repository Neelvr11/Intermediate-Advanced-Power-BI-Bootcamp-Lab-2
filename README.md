# Intermediate-Advanced-Power-BI-Bootcamp-Lab-2-Data Transform/ Cleaning
Skillsoft - Data Society 4 day Intermediate/Advanced Power BI Bootcamp.

# 1) Impot and clean the sales target table so that is in a usable format for data modelling

Import Power Cycle Sales Target.xlsx file.

From the Home Table and utilize the remove rows option to remove unused rows

![image](https://github.com/user-attachments/assets/13687188-7f03-476a-a011-104bdfe26c08)

From the Transform tab you can select “Use First Row as Headers” to promote the first row to the table header

Change the data type in the EmployeeID column from test to whole number	 

# 2) Unpivoting the date columns to rows 

Select the Employee column then navigate to the Transform tab and select from the unpivot drop-down unpivot other columns	

![image](https://github.com/user-attachments/assets/b344c3d5-1d81-47f7-9145-9b09dd153c14)

![image](https://github.com/user-attachments/assets/9a854326-b880-4815-9000-54d8c05f9f10)

Change the Value column to a fixed decimal data type.

![image](https://github.com/user-attachments/assets/971f06e9-3db6-4735-87df-73a457f6f7a7)

From the Transform tab select replace values -> replace errors and replace the errors with “0”

![image](https://github.com/user-attachments/assets/96282b7b-a728-4d43-a1ec-c90fc3037891)

Rename the Value column to Sales Target	

# 3) Column by example 

From the Add Column tab select the Column From Example

Select the check box on the Attribute column.

Enter the Month – 1-Year as the example in the Custom column first cell * note that for the AI engine to generate the subsequent values you might need to input 2-3 examples.

![image](https://github.com/user-attachments/assets/e9b673e1-3aa9-4e88-9d0f-6b79684e31a6)

Change the custom column data type from text to Date type and rename the column to Date.

Remove the Attribute column.

# 4) Create Grouping for Sale Target 

From the Transform tab select Group By

![image](https://github.com/user-attachments/assets/1ed8b639-53f4-4950-b9a4-f4de43d95409)

You will need to group by the date and title the new column name “Sale Target.”

![image](https://github.com/user-attachments/assets/6156939f-36e7-449c-936d-a9f47b220f1f)

The operation should be set to Max so that the group aggregation is taking the max value for the proposed target value.

![image](https://github.com/user-attachments/assets/865e236d-9a19-4c0d-97c1-8f38fb2b254d)

