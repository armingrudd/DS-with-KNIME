# DS-with-KNIME
This repository is created for a "Data Science with KNIME" course.

Participatns should fork this repository and upload reqired assignment files after each session.

The Final Score for each assignment is calculated as described here: You have 100 points at first. For missing each task's main activity you lose 10 points and having minor mistakes reduces 5 points of your starting points.This will be your score as "Completeness" of assignment. After calculating the completeness of assignment, you lose 2.5% of your score for each extra commit you had (each time you amend your assignment after getting instructor's feedback so the instrucor checks your assignment again = 1 extra commit) and 0.5% for each hour you delayed doing the assignment. A "Bonus Score" will be added to your assignment score if there is something creative or interesting in your assignment (The assignment score may not exceed 100).

The Final Score will be the average of all the assignment scores.

Good luck.

----------

Session 2 Assignment: To complete this assignment you need to upload your workflow to your repository. The name of the file must be: \<githu username\>-session\<session number\>

Task 1: Create a workflow group named "DS-with-KNIME" under LOCAL mountpoint and put a folder named "data" inside workflow group. Then download the provided files in "data" folder of this repository and put them in the "data" folder under "DS-with-KNIME" in your KNIME workspace. Also create another workflow group named "session2" in "DS-with-KNIME" and create your workflow in this workflow group. You have to create new workflow groups for each session and name them this way (session\<session number\>).

Task 2: Read both "adult.csv" (2 times) and "cars-85.xlsx" files:

1- Read "adult.csv" with column headers and read the first 32000 rows only.

2- Read "adult.csv" and skip the first 32000 rows.

3- Read "cars-85.xlsx" with column headers. Skip the first 2 columns ("symboling" and "normalized losses") and read the first 201 rows.

4- Read "cars-85.xlsx" with column headers. Skip the first 2 columns ("symboling" and "normalized losses") and read the last 5 rows only.

Task 3: Write files to LOCAL>DS-with-KNIME>data:

1- The output of task2-1 as XLSX with column headers, the same file name as the input file and "part1" as the sheet name.

2- The output of task2-2 as XLSX with the same file name as the input file and "part2" as the sheet name. After completing this task, the output file must have 2 sheets (part1 and part2).

3- The output of task2-3 as CSV with column headers and the same name as the input file.

4- The ouput of task2-4 as CSV with column headers and the same name as the input file. After completing this task, the row count of the output file must be the same as the row count of the input file (cars-85.xlsx).
