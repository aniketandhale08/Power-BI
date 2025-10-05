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
1. **New column**(Calculated column): Based on existing columns, you want to create new column. each rows will have record and this column will present physically in data model. 
2. **New Measure**: Based on existing columns, If you want to create a single calculated value from any existing column (values like, sum) this column will **not** present physically in data model. you can able to use it while creating visuals by draging from data panal. measures are mainly used for creating a single value or can say to use them in KPIs.
   
**DAX Syntax:**
   column name/ measure name= function(table name[column])
   - function: sum, count, average, if, etc
   - table name: name of table where that column is present
   - column: name of column of which you want to create a measure

**Some functions in Power BI:**
1. **Date and Time functions**: Functions for working with date and time values, such as DATE, NOW, and YEAR.
2. **Text functions**: Functions for working with text values, such as CONCATENATE, LOWER, and UPPER.
3. **Information functions**: Functions for obtaining information about values and data types, such as ISTEXT and ISNUMBER.
4. **Filter functions**: Functions for filtering data based on conditions, such as FILTER and CALCULATETABLE.
5. **Aggregation functions**: Functions for aggregating data, such as SUM, AVERAGE, and COUNT.
6. **Time Intelligence functions**: Functions for working with time-based data, such as SAMEPERIODLASTYEAR and TOTALYTD.
7. **Logical functions**: Functions for working with logical values and conditions, such as IF and SWITCH.
8. **Lookup functions**: Functions for looking up values in related tables, such as LOOKUPVALUE and RELATED.
9. **Math and Trigonometry functions**: Functions for performing mathematical calculations, such as ABS and SIN.
10. **Statistical functions**: Functions for working with statistical data, such as STDEV and PERCENTILE.
11. **Financial functions**: Functions for performing financial calculations, such as NPV and IRR.
12. **Other functions**: Functions that don't fit into the above categories, such as NOW and GUID.
















02:00 timestamp
