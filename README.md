## Power Query Transformation: Logistics Operations Data

This project demonstrates the use of Power Query to transform and prepare logistics operations data. The main task was to load raw data into Power BI and create a clear, structured table for analysis. The requirements specified the following:

### Task Requirements:
1. Load the data into Power BI and create a table with the following fields:
   - **Vehicle Number**  
   - **Task** 
   - **Starting Point**  
   - **End Point**  
   - **Start Date (Planned)**   
   - **End Date (Planned)**   
   - **Duration**   
   - **Driver**   
   - **Trip**   
   - **Shift**   
   - **Carrier**   

   The table should include only the tasks that were not marked as "Cancelled".

2. Create a new table that displays the total duration for each trip.

### Data Transformation Process:
Using Power Query, the data was transformed as follows:
- Filtered out tasks with a "Cancelled" status to include only completed or ongoing tasks.
- Structured the table according to the specified fields for a clear and easy-to-analyze format.
- Created a second table summarizing the total duration of each trip using grouping and aggregation functions.
  
Additionally, several key transformations were applied to achieve the final structure:

#### Splitting Column by Delimiter
The "Column1" field contained vehicle information that needed to be split into two separate fields for clarity. The column was split using the `#` delimiter.

**M Code:**
```M
= Table.SplitColumn(#"Changed Type", "Column1", Splitter.SplitTextByEachDelimiter({"#"}, QuoteStyle.Csv, true), {"Column1.1", "Column1.2"})
