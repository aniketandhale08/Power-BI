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

#### Some functions in Power BI:
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


### Text Functions in DAX

**1. LEFT**: Returns the specified number of characters from the start of a text string.
**2. LEN**: Returns the number of characters in a text string.  
**3. LOWER**: Converts all letters in a text string to lowercase.  
**4. MID**: Returns a string of characters from the middle of a text string, given a starting position and length.  
**5. REPLACE**: Replaces part of a text string with a different text string.  
**6. REPT**: Repeats text a given number of times. Use REPT to fill a cell with a number of instances of a text string.  
**7. RIGHT**: Returns the specified number of characters from the end of a text string.  
**8. SUBSTITUTE**: Replaces existing text with new text in a text string.  
**9. COMBINEVALUES**: Combines the given set of operands using a specified delimiter.  
**10. CONCATENATE**: Joins two text strings into one text string.  
**11. CONCATENATEX**: Evaluates expression for each row on the table, then returns the concatenation of those values in a single string result, separated by the specified delimiter.  
**12. EXACT**: Checks whether two text strings are exactly the same and returns TRUE or FALSE. EXACT is case-sensitive.  
**13. FIND**: Returns the starting position of one text string within another text string. FIND is case-sensitive and accent-sensitive.  
**14. FIXED**: Rounds a number to the specified number of decimals and returns the result as text with optional commas.  
**15. FORMAT**: Converts a value to text in the specified number format.  
**16. TOJSON**: Converts the records of a table into a JSON text.  
**17. TRIM**: Removes all spaces from a text string except for single spaces between words.  
**18. UNICHAR**: Returns the Unicode character that is referenced by the given numeric value.  
**19. UNICODE**: Returns the number (code point) corresponding to the first character of the text.  
**20. UPPER**: Converts a text string to all uppercase letters.  
**21. VALUE**: Converts a text string that represents a number to a number.  
**22. TOCSV**: Converts the records of a table into a CSV (comma-separated values) text.

### Logical function in DAX

**1. IF**: Returns a value based on a specified condition. The syntax is IF(condition, [value_if_true], [value_if_false]).
**2. AND**: Returns TRUE if all its arguments are TRUE, and returns FALSE otherwise. The syntax is AND(condition1, [condition2], ...).  
**3. OR**: Returns TRUE if any of its arguments are TRUE, and returns FALSE otherwise. The syntax is OR(condition1, [condition2], ...).  
**4. NOT**: Reverses the logical value of its argument. The syntax is NOT(condition).  
**5. SWITCH**: Returns a value based on the first TRUE expression. The syntax is SWITCH(expression, value1, result1, [default or value2, result2], ...).  
**6. IFERROR**: Returns the first argument if it is not an error value, otherwise it returns the second argument. The syntax is IFERROR(value, value_if_error).  
**7. IFNA**: Returns the first argument if it is not the #N/A error value, otherwise it returns the second argument. The syntax is IFNA(value, value_if_NA).


### Types of operators in DAX

**1. Arithmetic Operators**: Used to perform arithmetic operations such as addition (+), subtraction (-), multiplication (*), and division (/).
**2. Comparison Operators**: Used to compare values and return a logical result (TRUE or FALSE). These include equal to (=), not equal to (<>), greater than (>), less than (<), greater than or equal to (>=), and less than or equal to (<=).  
**3. Logical Operators**: Used to perform logical operations such as AND, OR, and NOT.  
**4. Concatenation Operators**: Used to combine text values, such as & and CONCATENATE.  
**5. Reference Operators**: Used to reference cells or ranges, such as [] and [].  
**6. Parenthesis**: Used to control the order of operations in a formula, such as () and [].  
**7. Miscellaneous Operators**: Used for various purposes, such as the colon (:) operator used in date and time functions and the semicolon (;) operator used in the SWITCH function.


**Card & KPI**

1. **Card:** Displays a single value like total sales or number of customers. Best for showing simple, standalone metrics without comparisons.
2. **KPI:** Compares a current value to a target or previous value with visual cues. Ideal for tracking performance trends and progress toward goals.



**Tooltips**
- They are mainly used for showing more details about the chart; by hovering over the chart, you can view the chart that you created in tooltips.
- enhance interactivity by displaying additional context or visuals when users hover over data points, helping to keep reports clean while offering deeper insights.  
- You need to create a new page where you will design the charts that will be shown as tooltips.


#### Some add on things
1. Tool Tips in Power BI
2. Bookmarks and Buttons






02:00 timestamp
