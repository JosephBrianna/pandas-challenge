
# PyCity Schools Analysis

In this analysis, we delved into the academic performance of students from various schools in the PyCity School District. Our primary data sources are two CSV files: one containing school information (`schools_complete.csv`) and the other containing student information (`students_complete.csv`).

## Setup and Data Loading

The necessary dependencies for this analysis include:

```python
import pandas as pd
from pathlib import Path
```
##terminal
pip install pandas
pip install pathlib

The data from the CSV files are loaded into DataFrames, and subsequently, the student and school data are merged based on the `school_name` column.

## District Summary

We began by providing an overview of the school district's metrics:

1. Total number of unique schools
2. Total number of students
3. Total budget for the entire district
4. Average math score
5. Average reading score
6. Percentage of students passing math (with a score >= 70)
7. Percentage of students passing reading
8. Overall passing rate (i.e., students who passed both math and reading)

The results are consolidated into a `district_summary` DataFrame.

## School Summary

The next section of the analysis breaks down performance metrics by individual schools:

1. Type of school (District or Charter)
2. Total number of students per school
3. Total budget per school and per capita spending per student
4. Average math and reading scores
5. Percentage of students passing math and reading
6. Overall passing rate by school

The findings are gathered in the `per_school_summary` DataFrame.

## Performance Analysis

1. **Highest-Performing Schools (by % Overall Passing)**: This section sorts schools based on the highest overall passing rate.
   
2. **Bottom-Performing Schools (by % Overall Passing)**: Conversely, this segment sorts schools based on the lowest overall passing rate.

3. **Math and Reading Scores by Grade**: Here, we segregate scores based on grade level for each school.

4. **Scores by School Spending**: Schools are categorized into spending brackets based on the budget per student. Metrics like average scores and passing rates are analyzed per bracket.

5. **Scores by School Size**: We categorize schools into small, medium, and large based on their student population. Similar to the spending analysis, we then assess academic performance metrics.

6. **Scores by School Type**: Finally, schools are grouped by type (District or Charter), and their performance metrics are averaged.

---

## Conclusion

This analysis offers stakeholders an extensive view of the academic performance across various schools in the PyCity School District. By examining different metrics, decision-makers can make informed choices about allocating resources, implementing interventions, or adopting best practices from top-performing schools.
