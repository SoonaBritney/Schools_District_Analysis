# Schools_District_Analysis


Student Name: Soona Britney Cheon
Date: 10/16/2020
Module 4 Challenge

TITLE: School Distrcit Analysis
1. Overview of the school district analysis: 

A. PURPOSE
The purpose of the Scholl District Analysis is analying the below:
1) Data Cleaning: Due to the dishonesty among the Thmoas High School 9th graders' math and reading score, we will selectivly remove the the Thmoas High School 9th graders' math and reading scores from the data for accurate School Disctrict Analysis 
2) School Summary: It consists the scnapshot of the schools: such as school size, school type, student id, student name, number of students in per school, school budget size, and most importantly math scores and reading score of each student, which we can analyze as the major performance and comparison among schools. 
3) High and Low Performance Schools - based on the math and reading score performace, we will find the top 5 and bottom 5 performers in the district. 
4) Math and Reading Scores by Grade in the school ditrict: we will analyze the math and reading scores to find out the below
 - average score of math as a whole school distrcit, average score of math per school, count of students who scored over 70 in math (passed), percentage of students who scored over 70 in math (passed rate) 
 - average score of reading as a whole the school distrcit, average score of reading score per school, count of students who scored over 70 in reading (passed), percentage of students who scored over 70 in reading (passed rate)   
5) Scores by School Spending we will analyze the school budget by per individual student to measure how much school budget is ideal for stuent's best academic performance 
6) Scores by School Size - we will analize the school size and students' academic pefromance to find out the ideal school size for the best academic performance for students 
7) Scores by School Type -we will analize the school type and students' academic pefromance to find out the ideal school size for the best academic performance for students 

B. Background
The school board has notified Maria and her supervisor that the students_complete.csv file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards and have turned to Maria for help. She has asked you to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Once you’ve replaced the math and reading scores, Maria would like you to repeat the school district analysis that you did in this module and write up a report to describe how these changes affected the overall analysis.

SCREENSHOT:
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/THS_9_NaN.PNG?raw=true

C. Results: 
(Using bulleted lists and images of DataFrames as support, address the following questions.)

0) Data Cleaning: In the school ditrcit, 
- we have 15 schools from greade 9th to 12th.  
- the total number of students in the school distrct is 39,170, 11,408 students in 9th grade in the scenario, we have 461 students in the Thomas High School at 9th gread, who was academically dishonest, and could nuse the math and reading scores in the analysis. 
- the student size per school is as below
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/per_school_counts.PNG
- This is 1.17% of the total students, and 4.04% of the total 9th graders in the school district. Thus, this dropped out data of Thomas High School 9th graders will impact the 9th graders performance analysis.

1) How is the district summary affected?
- The number of the students in the Thomas High School 9th grade are 461, this group's (THS_9) average reading score is 83.72, average math score is 83.59.
- Meantime, the total number of the school district is 39,170 including THS_9 students, and 38,709 excluding the THS_9 students. When exclude the THS_9 students from the total, the average reading score is 81.86, average math score is 78.93.
- It means, if we included the THS_9's dishonest math and reading scores, the overall average reading and math score would be up.  
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/district_summary.PNG


2) How is the school summary affected?
- We analyzed the school summery per school, and here is the summary
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/per_school_summary.PNG


3) How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
- the 9th grade students in Thomas High School is analyzed as below.  

4) How does replacing the ninth-grade scores affect the following:

5) Math and reading scores by grade
Here is the reading scores per grade in the district 
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/reading_per_grade.PNG
here is the math scores per grade in the district
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/math_scores_by_grade.PNG

6) top 5 schools & bottom 5 schools
top 5 schools - https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/top_5_schools.PNG
bottom 5 schools - https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/bottom_5_schools.PNG

7) Scores by school spending
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/spending_summary.PNG

8) Scores by school size
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/school_size_analysis.PNG

9) Scores by school type
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/school_type_analysis.PNG

Summary: 
Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/THS_9_NaN.PNG?raw=true

Deliverable 3 Requirements
Structure, Organization, and Formatting (7 points)
The written analysis has the following structure, organization, and formatting:

There is a title, and there are multiple sections (2 pt).
Each section has a heading and subheading (3 pt).
Links to images are working, and code is formatted and displayed correctly (2 pt).
Analysis (18 points)
The written analysis has the following:



Overview of the school district analysis:

The purpose of this analysis is well defined (3 pt).
Results:

There is a bulleted list that addresses how each of the seven school district metrics was affected by the changes in the data (10 pt).
Summary:

There is a statement summarizing four major changes to the school district analysis after reading and math scores have been replaced (5 pt).
