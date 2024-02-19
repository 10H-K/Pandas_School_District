# Utilizing Pandas to Analyze School and Standardized Test Data

## Overview ##

The objective of this project is to help relevant authorities, such as the school board and mayor, make strategic decisions regarding future school budgets and priorities. To accomplish this, the created Jupyter Notebook analyzes the district-wide school data, which includes every student's math and reading scores along with various information on the schools they attend, to reveal trends in school performance.

## Process ##

A) Setup:
  1. Importation of dependencies (Pandas and Path)
  2. Setting file path to target csv files (school data and student data)
  3. Reading both csv data files, storing into Pandas DataFrames
  4. Combination of DataFrames into single DataFrame

B) District Summary: district's key metrics for budget and student performance
  1. Calculation of total number of unique schools in the district
  2. Calculation of total number of students in the district
  3. Calculation of total budget for the district
  4. Calculation of average math score for the district
  5. Calculation of average reading score for the district
  6. Calculation of percentage of students in the district that passed the math section (defined as math score greater than or equal to 70)
  7. Calculation of percentage of students in the district that passed the reading section (defined as reading score greater than or equal to 70)
  8. Calculation of percentage of students in the district that passed the math and reading sections
  9. Creation and formatting of DataFrame displaying high-level snapshot of the district's key metrics

C) School Summary: key metrics associated with each individual school
  1. Capture of unique school names and corresponding types (District or Charter)
  2. Calculation of total student count for each school
  3. Calculation of total budget and per capita spending for each school
  4. Calculation of average test scores per school
  5. Calculation of number of students per school that passed the math section
  6. Calculation of number of students per school that passed the reading section
  7. Calculation of number of students per school that passed the math and reading sections
  8. Calculation of overall passing rates per school
  9. Creation and formatting of DataFrame displaying key metrics associated with each school

D) Highest Performing Schools: ranking by overall passing percentage
  1. Sorting individual schools by overall passing percentage in descending order, displaying top 5 schools

E) Lowest Performing Schools: ranking by overall passing percentage
  1. Sorting individual schools by overall passing percentage in ascending order, displaying top 5 schools

F) Math Scores by Grade: calculated for each individual school
  1. Separation of data by grade levels, calculation of average math scores for each grade level, creation and formatting of DataFrame displaying average scores for each school

G) Reading Scores by Grade: calculated for each individual school
  1. Separation of data by grade levels, calculation of average reading scores for each grade level, creation and formatting of DataFrame displaying average scores for each school

H) Scores by School Spending: breakdown of student performance based on school spending per capita
  1. Establishment of spending bins and associated labels
  2. Creation of school summary DataFrame copy
  3. Utilization of `pd.cut` for categorization of school spending based on bins
  4. Calculations for average student performance based on spending bins/labels
  5. Creation and formatting of DataFrame displaying student performance district wide based on spending bins/labels

I) Scores by School Size: breakdown of student performance based on school size
  1. Establishment of size bins and associated labels
  2. Utilization of `pd.cut` on "Total Students" column of the school summary DataFrame
  3. Calculations for average student performance based on size bins/labels
  4. Creation and formatting of DataFrame displaying student performance district wide based on size bins/labels

J) Scores by School Type: breakdown of student performance based on school type
  1. Calculations for average student performance based on school type (District or Charter)
  2. Creation and formatting of DataFrame displaying student performance district wide based on school type

