## Steps to follow in data transformation
1. Name the tables after importing
2. Use the first row as a header
3. Deal with Null values/ make actuals in the column if they are not (format: null), use the replace function.
4. Remove unwanted columns
5. Data type
6. Remove duplicate
7. Date transformation (Year, months, weeks, days)
8. Merge columns/ Split columns/ Trim
9. Change the order/ sequence of columns
10. Make format same for all dates.
    right click on column--> chnage type--> using local--> select date as datatype--> select required locale.

#### Further steps:
1. Calculate the count of days in  between two dates using tab Add column--> Custom column
2. Add column--> Duration (Weeks, Days, Hours, minute)
3. Adding Conditional Columns to Power BI
4. Merge Queries and Append Queries in Power BI (get column from another table, merge same table data in stack like form)
5. Check newely creaetd columns data types/format
6. Pivoting and Unpivoting of Data in Power BI
- to transpose the table data use this feature "Unpivot other columns"
- using this, lenthy table will get shrink to small table with proper data readability.
- Using "Pivot table" fiunction make table more readable.


## Steps to follow in data modelling
1. Managing Data Relationships
   - to make relationship betwwen table you can view the 3rd tab "Model View", here you can see the diagram of data model.
   - to make relationship between two tables find the common column smong them.
2. Understood the cardinality of data model of your report.
3. Make selection of Cross-Filter Direction.



## DAX (Data Analysis Expressions)
**New column & New Measure**
1. New column: Based on existing columns, you want to create new column. each rows will have record and this column will present physically in data model.
2. New Measure: Based on existing columns, If you want to create a single calculated value from any existing column (values like, sum)


















02:00 timestamp
