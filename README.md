# School_District_Analysis
Replace ninth-grade reading and math scores and repeat the school district analysis
# Deliverable 1: Replace Ninth-Grade Reading and Math Scores (50 points)
Deliverable 1 

Using the Pandas loc method with conditional statements and comparison and logical operators, select the ninth-grade reading and math scores for Thomas High School. Then, use the Pandas NumPy module to change the reading and math scores to NaN.
Use the code snippet provided in Step 1 to import the NumPy module: import numpy as np.

1. Use the code snippet provided in Step 2 for the Pandas loc method.

2. To select all the ninth-grade reading scores at Thomas High School, use the following steps to write code inside the brackets of the loc method:

3. a) Add an opening parenthesis, then use a comparison operator to retrieve all the rows with Thomas High School from the "school_name" column of the student_data_df, then close the parenthesis.

b) Add a logical operator then another opening parenthesis, then use a comparison operator to retrieve all the rows with ninth grade from the "grade" column of the student_data_df, then close the parenthesis.

c) To change the reading scores only, add a comma after the last closing parenthesis then add the "reading_score" column.

d) Outside of the closing brackets of the loc method, set the ninth-grade reading scores from Thomas High School equal to np.nan.

![image](https://user-images.githubusercontent.com/107659667/179083006-45cefa56-ec70-487a-8368-b6e45b674689.png)
4. In Step 3, refactor the code from Step 2 to replace the math scores with NaNs.

5. In Step 4, check the student data to make sure the grades were replaced with NaNs.

6. After you run Step 4 in your PyCitySchools_Challenge_testing.ipynb file, confirm that the DataFrame looks like the image below, where the ninth-grade reading and math scores from Thomas High School have been replaced with NaNs. Then, make a copy of the PyCitySchools_Challenge_testing.ipynb file and rename it PyCitySchools_Challenge.ipynb.

![image](https://user-images.githubusercontent.com/107659667/179083247-9336f004-473f-43fb-98b2-263ac509193e.png)

# Deliverable 2: Repeat the School District Analysis

Repeat the school district analysis you did in this module, and recreate the following metrics:

 - The district summary
 - The school summary
 - The top 5 and bottom 5 performing schools, based on the overall passing rate
 - The average math score for each grade level from each school
 - The average reading score for each grade level from each school
 - The scores by school spending per student, by school size, and by school type
In Steps 1-4, you’ll update the district summary. For this task, you’ll recalculate the total student count by subtracting the number of ninth-grade students in Thomas High School from the total student count, then you'll recalculate the passing math and passing reading percentages, and the overall passing percentage with the recalculated total student count.

In Steps 5-14, you’ll execute the code from this module that creates and formats the School Summary DataFrame, then update the school summary using the 10th-12th graders from Thomas High School as follows:

 - First, you’ll calculate the number of 10th-12th graders in Thomas High School.

 - Create three new DataFrames for the 10th-12th graders from Thomas High School: students who passed math, students who passed reading, and students who passed both math and reading.
 
 - Using these DataFrames, you'll recalculate the percentage of students who passed math, passed reading, and passed both math and reading for Thomas High School only.

 - Finally, you'll replace the % Passing Math, % Passing Reading, and % Overall Passing scores in the current School Summary DataFrame with the new passing percentages for Thomas High School.

Use the instructions below to add code where indicated by the numbered-step comments in the starter code file to update the District Summary DataFrame.

1. In Step 1, using the loc method with logical and comparison operators, retrieve the student count for Thomas High School ninth graders in the school_data_complete_df DataFrame.
2. In Step 2, subtract the number of students retrieved from Step 1 from the total student count to get the new total student count.
3. In Step 3, calculate the math and reading passing percentages based on the new total student count.
4. In Step 4, calculate the overall passing percentage with the new total student count.
Before moving on, confirm that that your District Summary DataFrame looks like this image:

![image](https://user-images.githubusercontent.com/107659667/179083726-dbb91154-246a-4e9b-8d4b-52bd6c28acd8.png)

Use the instructions below to add code where indicated by the numbered-step comments in the starter code file to update the School Summary DataFrame.

5. Run the code from this module that creates and formats the School Summary DataFrame.
Before moving on, confirm that the metrics for Thomas High School look like this image.

![image](https://user-images.githubusercontent.com/107659667/179083881-321e2232-00bd-4744-80f4-f10bb70000ae.png)

6. In Step 5, get the number of 10th-12th grade students from Thomas High School.
7. In Step 6, use the loc method to create a new DataFrame that has all the students passing math from Thomas High School.
8. In Step 7, use the loc method to create a new DataFrame that has all the students passing reading from Thomas High School.
9. In Step 8, use the loc method to create a new DataFrame that has all the students passing math and reading from Thomas High School.
10. In Step 9, calculate the percentage of 10th-12th grade students passing math from Thomas High School.
11. In Step 10, calculate the percentage of 10th-12th grade students passing reading from Thomas High School.
12. In Step 11, calculate the overall passing percentage of 10th-12th grade students from Thomas High School.
13. In Step 12, use the loc method to replace the % Passing Math score for Thomas High School with the new math passing percentage you calculated in Step 9.
14. In Step 13, use the loc method to replace the % Passing Reading score for Thomas High School with the new reading passing percentage you calculated in Step 10.
15. In Step 14, use the loc method to replace the % Overall Passing score for Thomas High School with the new overall passing percentage you calculated in Step 11.

Before moving on, confirm that the updated metrics for Thomas High School look like this image:

![image](https://user-images.githubusercontent.com/107659667/179084228-6360b022-485b-41f9-bdf1-9315f054ac7a.png)

Next, complete the following steps for school district analysis using the remaining steps that are provided in the starter code.

 - The top 5 and bottom 5 performing schools, based on the overall passing rate
 - The average math score for each grade level from each school
 - The average reading score for each grade level from each school
 - The scores by school spending per student, by school size, and by school type

# Deliverable 3: A Written Report for the School District Analysis
1.	Overview of the school district analysis: Explain the purpose of this analysis.

The purpose of this analysis was to see any evidence of academic dishonesty specifically in reading and math grades for Thomas High School ninth graders, which appear to have been altered. In this study, we replaced the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Once we replaced the math and reading scores, we repeated the school district analysis.

The district went from 65% of overall passing to 54%.

![image](https://user-images.githubusercontent.com/107659667/179090394-dfa804ba-b94f-4c86-9edf-ccc94d4fcf6a.png)

![image](https://user-images.githubusercontent.com/107659667/179090420-e8f3d4c7-6d4d-46fc-a698-83054100bbb0.png)

The school summary was affected by decreasing the average passing rate of Thomas High school. They went from ranking 2nd in the district to 13th. Overall, the spending limits were increased and the passing rates of the ninth graders (and subsequently the district) was decreased.


