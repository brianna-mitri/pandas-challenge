# Pandas Challenge
Combine two datasets (student and school data), to analyze a school district's standardized test results for math and reading.

Then create and export dataframes to an Excel file (also displayed in the Jupyter notebook's outputs).

## Dataframes
The following dataframes are created from the original merged dataframe (*complete_df*):
- **District Summary** (*district_summary_df*): evaluates total schools and students in district, average scores and passing rates.
- **School Summary** (*per_school_summary_df*): evaluates each school's average scores and passing rates, and additional traits such as spending and total students.
- **Highest-Performing Schools by Percentage of Overall Passing** (*top_schools_df*): finds top 5 performing school based on overall passing rates.
- **Lowest-Performing Schools by Percentage of Overall Passing** (*bottom_schools_df*): finds lowest 5 performing school based on overall passing rates.
- **Math Scores by Grade** (*math_by_grade_df*): evaluates each school's average math scores based on grade level.
- **Reading Scores by Grade** (*read_by_grade_df*): evaluates each school's average reading scores based on grade level.
- **Scores by School Spending**: evaluates schools' spending ranges per student.
    - *school_spending_df*: School Summary dataframe plus added column with spending ranges per student
    - *spending_summary_df*: evaluates average scores and passing rates based on spending ranges per student.
- **Scores by School Size**: evaluates schools' sizes based on total students.
    - *school_size_df*: School Summary dataframe plus added column with small, medium, and large school size categories.
    - *size_summary_df*: evaluates average scores and passing rates based on school size categories.
- **Scores by School Type** (*type_summary_df*): evaluates average scores and passing rates based on school type (chater and district).

## Excel File Output
The following 5 sheets are created in the exported Excel file to categorize and display the values from the 12 dataframes made:
- **Overall School Data:** School Summary plus the two extra columns from *school_spending_df* and *school_size_df*
- **District Summary:** District Summary dataframe
- **School Performance:** Highest-Performing Schools by Percentage of Overall Passing and Lowest-Performing Schools by Percentage of Overall Passing
- **Scores by Grade:** Math Scores by Grade and Reading Scores by Grade
- **Scores by School Factors:** Scores by School Spending, Size, and Type dataframes

Column width and placement of the dataframes and titles on each sheet are dynamic depending on the dataframes' sizes. Below is an example of the output from the last sheet, **"Scores by School Factors"**, which clearly shows all 3 dataframes and their values:
![image-6](https://github.com/user-attachments/assets/68bce859-1e7b-46a8-aeaf-1ed271d61e70)

## Files
In order for the dataframes to be created and exported, the files are expected to be in the following format:
- **Output**[^1]
    - **PyCitySchools_Output.xlsx**: outputted Excel sheet containing summary dataframes
- **Resources**
    - **schools_complete.csv**: data about schools in the district
    - **students_complete.csv**: data about students in the district
- **PyCitySchools.ipynb**: where Python code is located and analysis (under "Findings")

[^1]: Output folder and excel sheet don't need to be created before running. The Jupyter notebook should generate them both.


