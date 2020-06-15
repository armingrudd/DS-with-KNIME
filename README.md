# DS-with-KNIME
This repository is created for a "Data Science with KNIME" course.

Participatns should fork this repository and upload reqired assignment files after each session.

The Final Score for each assignment is calculated as described here: You have 100 points at first. For missing each task's main activity you lose 10 points and having minor mistakes reduces 5 points of your starting points.This will be your score as "Completeness" of assignment. After calculating the completeness of assignment, you lose 2.5% of your score for each extra commit you had (each time you amend your assignment after getting instructor's feedback so the instrucor checks your assignment again = 1 extra commit) and 0.5% for each hour you delayed doing the assignment. A "Bonus Score" will be added to your assignment score if there is something creative or interesting in your assignment (The assignment score may not exceed 100).

The Final Score will be the average of all the assignment scores.

Good luck.

----------

Session 2 Assignment: To complete this assignment you need to upload your workflow to your repository. The name of the file must be: \<github username\>-session\<session number\>

Task 1: Create a workflow group named "DS-with-KNIME" under LOCAL mountpoint and put a folder named "data" inside workflow group. Then download the provided files in "data" folder of this repository and put them in the "data" folder under "DS-with-KNIME" in your KNIME workspace. Also create another workflow group named "session2" in "DS-with-KNIME" and create your workflow in this workflow group. You have to create new workflow groups for each session and name them this way (session\<session number\>).

Task 2: Read both "adult.csv" and "cars-85.xlsx" files:

1- Read "adult.csv" with column headers and read the first 32000 rows.

2- Read "adult.csv" and skip the first 32000 rows.

3- Read "cars-85.xlsx" with column headers. Skip the first 2 columns ("symboling" and "normalized losses") and read the first 201 rows.

4- Read "cars-85.xlsx" with column headers. Skip the first 2 columns ("symboling" and "normalized losses") and read the last 5 rows.

Task 3: Write files to LOCAL>DS-with-KNIME>data:

1- The output of task2-1 as XLSX with column headers, the same file name as the input file and "part1" as the sheet name.

2- The output of task2-2 as XLSX with the same file name as the input file and "part2" as the sheet name. After completing this task, the output file must have 2 sheets (part1 and part2).

3- The output of task2-3 as CSV with column headers and the same name as the input file.

4- The ouput of task2-4 as CSV with column headers and the same name as the input file. After completing this task, the row count of the output file must be the same as the row count of the input file (cars-85.xlsx).

----------

Session 3 Assignment: To complete this assignment you need to upload a Component which takes "adult" data set as input and produces a view as described in assignment tasks:

Task 1: Assigns colors to rows based on "marital-status".

Task 2: A table view which publishes selection events but does not subscribe to selection events.

Task 3: A table view which subscribe to selection events but does not publish selection events. Also, this table view only shows selected rows.

Task 4: A scatter plot which shows "age" against  "hours-per-week" for 1000 rows only.

Task 5: A bar chart which shows average "age" per "marital-status".

Task 6: A histogram which shows average "hours-per-week" per age groups. There should be 10 age groups. The label of each group must represent the borders.

Task 7: Design the Component layout in a way that the scatter plot, the bar chart and the histogram appear in the same row. Max height for table views should be 400 px.

Task 8: Add a workflow annotation inside the component and answer these questions:

1- In what age spans do we have the min and the max hours-per-week?

2- What is the average age of the people with "Never-married" and "Widowed" marital-status?

3- Do you see anything strange in the histogram ("hours-per-week" per age groups)? How do you explain it?

----------

Session 4 Assignment: To complete this assignment, you have to upload a workflow which reads "CallsData.xls" and "ContractData.csv" files and outputs the "session4-output.table" file.

----------

Session 5 Assignment: Upload a workflow and do the following tasks:

1- Read "cars-85".

2- Add the digit form of the number of doors (nr_doors) in front of the car's brand name (make) where the first 2 and the last character of the brand name are uppercased. E.g. MAzdA(4), VOlkswageN(2)

3- If the fuel price is 2$ per liter for gasoline and 2.5$ for diesel: for each car, calculate the distance (in kilometers) a person can drive in average (city and highway) if he/she can spend money equal to the car's price. Hint: 235/mpg=Lp100km

-----------

Session 6 Assignment: Upload a workflow which reads session6-assignment.table and outputs adult.csv (must be exactly the same in terms of cell values, row/column order, column names, column types, ...). You may use education-num.table in your workflow.

----------

Session 7 Assignment: Using the first 3000 rows of "CallsData.xls" and "ContractData.csv" files:

1- Build a classification model which predicts customer churn. Apply any preprocessing if needed.

2- Cluster customers based on customer service calls and charges (day, eve, night, intl). Apply any preprocessing if needed.

3- Using the clustering model in task 2, assign clusters to the remaining 333 customers.

----------

Session 8 Assignment: By using the "Market-Basket.table" data set, build and upload a workflow which recommends 2 products based on this basket: [onions, tomato, egg]. Design a scoring system to select the most beneficial rules.

----------

Session 9 Assignment: By using World Bank APIs and the "session9.sqlite" file upload a workflow:

Task 1: Get ID, name and region of all countries (exclude aggregates).

Task 2: Get total, urban and rural population of all countries in 2018 (exclude aggregates).

Task 3: Create 2 table in sqlite database (session9.sqlite): one for general info (ID, name and region) and one for population info. Use an integer value as the key to link tables. Hint: The population info table must have 4 columns; 3 columns for population info and the 4th column should be an integer key that specifies the corresponding country in general info table.

Task 4: Using the tables in the database: (Use in-database processing)

1- Aggregate values and calculate sum of total population for each region.

2- Filter countries where region is "Middle East & North Africa" and total population is >50 M.

Task 5: Read the output of Task 4 and for each country calculate % of region population.
