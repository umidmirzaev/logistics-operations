## Power Query Transformation: Logistics Operations Data

This project demonstrates the use of Power Query to transform and prepare logistics operations data. The main task was to load raw data into Power BI and create a clear, structured table for analysis. The requirements, initially provided in Russian, specified the following:

### Task Requirements:
1. Load the data into Power BI and create a table with the following fields:
   - **Vehicle Number** (Номер авто)
   - **Task** (Работа)
   - **Starting Point** (Точка начала)
   - **End Point** (Точка окончания)
   - **Start Date (Planned)** (Дата начала (план))
   - **End Date (Planned)** (Дата окончания (план))
   - **Duration** (Длительность)
   - **Driver** (Водитель)
   - **Trip** (Рейс)
   - **Shift** (Смена)
   - **Carrier** (Перевозчик)

   The table should include only the tasks that were not marked as "Cancelled" (не «Отменены»).

2. Create a new table that displays the total duration for each trip.

### Data Transformation Process:
Using Power Query, the data was transformed as follows:
- Filtered out tasks with a "Cancelled" status to include only completed or ongoing tasks.
- Structured the table according to the specified fields for a clear and easy-to-analyze format.
- Created a second table summarizing the total duration of each trip using grouping and aggregation functions.

### Screenshots:

**Raw Data Transformation (Before):**
![Dataset Overview](path-to-your-dataset-overview-image)

**Transformed Table (After):**
![Final Table 1](path-to-your-final-table-1-image)

**Summary Table of Total Duration per Trip:**
![Final Table 2](path-to-your-final-table-2-image)

These steps showcase the use of Power Query to filter, structure, and aggregate logistics data, resulting in a dataset ready for further analysis.
