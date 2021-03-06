# Schools_District_Analysis

Student: Soona Britney Cheon
Date: 10/16/2020
Module 4 Challenge

TITLE: School Distrcit Analysis
1. Overview of the school district analysis: 
=============================================================================

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

================================================================================

B. Background

The school board has notified Maria and her supervisor that the students_complete.csv file shows evidence of academic dishonesty; 
specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards and have turned to Maria for help. She has asked you to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Once you’ve replaced the math and reading scores, Maria would like you to repeat the school district analysis that you did in this module and write up a report to describe how these changes affected the overall analysis.


NaN SCREENSHOT:
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/THS_9_NaN.PNG?raw=true

==============================================================================
C. Results: 
(Using bulleted lists and images of DataFrames as support, address the following questions.)

0) Data Cleaning: In the school ditrcit, 

- we have 15 schools from greade 9th to 12th in the district.   
- the total number of students in the school distrct is 39,170, 11,408 students in 9th grade in the scenario, we have 461 students in the Thomas High School at 9th gread, who was academically dishonest, and could nuse the math and reading scores in the analysis. 
- the average reading score cross schools in the distrcit is 81.87, while average math score is 78.98. It means students' performance is better in the reading subject.  
- the student size per school is as below
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/per_school_counts.PNG
- This is 1.17% of the total students, and 4.04% of the total 9th graders in the school district. Thus, this dropped out data of Thomas High School 9th graders will impact the 9th graders performance analysis.

==============================================================================

1) How is the district summary affected?
Due to the Academic dishonesty, we decided to make the Thomas High School Students math and Reading scores as NaN

(1) The number of the students in the Thomas High School 9th grade is 461 among total 1635 students in the Thomas High School, This group's (THS_9) average reading score is 83.84, average math score is 83.59, which is higher than the average score in the district. However, when we compared the average scores of the 10th, 11th, 12th grade students in the Thomas High School, it was almost same level. Althouhg, if we make the THS 9th grader's reading and math scores as NaN, recalculate the average, the average reading score in Thomas High School was went up (83.85 ==>83.89), and the average math score actually went down (83.41 ==> 83.35). Thye assumption is, if the THS 9th greade students were dishonest, prabably, they did more in math.  
(2) Meantime, the total number of the school district is 39,170 including THS_9 students, and 38,709 excluding the THS_9 students. When exclude the THS_9 students from the total, the average reading score is 81.86, average math score is 78.93.
(3) It means, if we included the THS_9's dishonest math and reading scores, the overall average reading and math score would be up.  

Disticrt summary before cleaning THS_9 dishonest data
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/dictrict_summary_before_clean_THS_9.PNG

District summary after cleaning THS_9 dishonest data as NaN
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/district_summary.PNG

BEFORE AD AFTER WE CHNAGE Thomas High School 9th Grade students data to Nan

BEFORE WE DROP THS_9 record as NAN ========> AFTER WE DROP THS_9 records as NAN
========================================================================================
(1)Total Schools	15 ========> 15 (Analysis: it is school data specific, so there is no impact)

(2)Total Students	39,170 ========> 38,709 (Analysis: the total student is decreaed for 461, which will impact the average score, school budget per capital, school performance per School size, School performance per grade, etc. will impact the entire analysis. )

(3)Total Budget	$24,649,428.00 ========> $24,649,428.00 (Analysis: it is same but if we drop the student account, it will misinform that per student school budget spnding will look like increaesed, and it is not true.)

(4) Average Math Score	79.0 ============> 78.9 (Analaysis: When we included the Thomas High School (THS) 9th score as was, the average math score was 0.1% highr before. It could be a good evidence, the academic performance was dishonest for THS 9th grade students in math.)

(5) Average Reading Score		81.9 ============> 81.9 (Analysis: it looks like same, but it is calculated per new total student account, 38,709.)

(6) % Passing Math	75.0 ============> 74.8  (Analaysis: When we included the Thomas High School (THS) 9th score as was, the % Passing Math was 0.2% highr before. It could be a good evidence, the academic performance was dishonest for THS 9th grade students in math.)

(7)% Passing Reading		85.8 ===========>  85.7 (Analaysis: When we included the Thomas High School (THS) 9th score as was, the % Passing Reading was 01.% lower before. It could be a good evidence, that THS 9th greade students are not actully outprrforming group. It concerns the data quality and realiability & validity of the School Analysis.)

(8) % Overall Passing 65.2 =============>  64.9 (Analaysis: Once again, When we included the Thomas High School (THS) 9th math and reading scores as was, % Overall Passing as was 0.3% higher before. It could be a good evidence, the academic performance was dishonest for the THS 9th grade students in math.)

========================================================================

2) How is the school summary affected?
- We analyzed the school summery per school, and here is the summary
school analysis summary
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/school_summary.PNG

school analysis summary per school
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/per_school_summary.PNG

- In the school district, we have 15 schools, 38,709 students, total budget is $24,649,428.00, Average Math Score is 78.9, 	Average Reading Score is 81.9, 
% Passing Math is 85.7%, % Passing Reading	is 85.7%, and finally the % Overall Passing is 64.9%.
The school ditrict should focus on improving academic performance in math in general.
- if we remove the THS 9th grade students scores, the outcome was not significantly altered. In fact, the dishonest math and reading scores of 461 THS_9th gradee studnts data needed to be NaN, and it altered the analsis in every aspects.  
========================================================================

3) How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
- the 9th grade students in Thomas High School is analyzed as below.  
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/school_summary.PNG

4) How does replacing the ninth-grade scores affect the following:
(1)THS_9 Math and Reading scores became NaN:
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/THS_9th_Grade_Math_Reading_NaN.PNG
(2) The math and reading scores became lower after THS_9 dishonest scores cleaned up.

5) Math and reading scores by grade
Here is the reading scores per grade in the district (showing NaN for THS_9th grade) 
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/reading_per_grade.PNG
here is the math scores per grade in the district
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/math_scores_by_grade.PNG

===============================================================================

6) top 5 schools & bottom 5 schools
Here are the results:
top 5 schools - https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/top_5_schools.PNG
bottom 5 schools - https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/bottom_5_schools.PNG

==================================================================================

7) Scores by school spending
The outcome is as below.
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/spending_summary.PNG
The finding is vey interesting, that the school spending per school was not significatly improve the school performance. 

=================================================================================

8) Scores by school size
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/school_size_analysis.PNG
When we compared the Average Math Score, Average Reading Score,	% Passing Math,	% Passing Reading, % Overall PassingThe analysis compared with school size, it shows that when the school size is smaller, the academic performance was better.
The best performance: Small (<1000) school size	> 
The second best performance: Medium (1000-2000)	> 
The least performance: Large (2000-5000)

=============================================================================

9) Scores by school type
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/school_type_analysis.PNG

It is very obvious that chartet school performed significatly better in the below academic performance. Especially, math performance was significantly successful. 

School Type					
Charter	- Average Math Score:83.5, 	Average Reading Score:83.9,		% Passing Math:90,	% Passing Reading:93	% Overall Passing:87%
District	- Average Math Score:77.0	Average Reading Score: 81.0,	% Passing Math:67,	% Passing Reading: 81	% Overall Passing:54%

Concluion:
==============================================================================

As we analysize the data after changed the math and reading scores of the Thomas High School at 9th grade, we are experiencig a significant realiability and validity issue with the data quality, and analysis outcome.
As we can see below, the altered 461 student's math and reading scores shows the strong evidence of academic dishonesty in reading and math, specifically % math passed rate, and average math score. 

(1) Data Cleaning: Thomas High School 9th grade students math and reading scores are obvioously high than it was supposed to be. After we dropped these scores as NaN, the average, and the count of passed math & reading, % of passed math reading has lowed. ==> it was a proper idea to made this groups test score as NaN.
(2) School Summary: After THS_9th grade students scores are treated as Nan, the snapshot of schools, students list, student count, and the most importantly math scores and reading scores of average, count of passed, % of passed students in math and reading became lower. 
3) High and Low Performance Schools - as below
- top 5 schools (Cabrera Hish School was the best school in the school district)
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/top_5_schools.PNG
- bottom 5 schools (The Rodriguez High school was the worst in academic standard point)
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/bottom_5_schools.PNG

4) Math and Reading Scores by Grade in the school ditrict: we will analyze the math and reading scores to find out the below
 - math scores per grade (THS_9 matjs score shows as NaN) - it became lower than before since dishonest scores were treated as NaN
 https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/math_scores_by_grade.PNG
 
 - reading scores per grade (THS_9 matjs score shows as NaN) - it became lower than before since dishonest scores were treated as NaN
 https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/reading_per_grade.PNG
 
5) Scores by School Spending - the school spnding er capita was not a significant factor to improve students academic performance. 
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/spending_summary.PNG

6) Scores by School Size - the smaller school size is better for academic performance
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/school_size_analysis.PNG

7) Scores by School Type - the charter school was better for school academic performance
https://github.com/SoonaBritney/Schools_District_Analysis/blob/main/screenshots/school_type_analysis.PNG


THnak you.





