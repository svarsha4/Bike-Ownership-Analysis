
<!-- README.md is generated from README.Rmd. Please edit that file -->

# Bike Ownership Analysis

## By: Saul Varshavsky

<!-- badges: start -->
<!-- badges: end -->


### Project Description

This project aims to create a dashboard to visualize how bike ownership is related with levels of income and commute distance to work.


### Core Aspects of the Project

- **Data Cleaning**:
  - Refer to the *Data Sheet* worksheet in the Excel workbook
  - All duplicates were removed.
  - **Find and Replace** was used for the "Marital Status" and "Gender" columns. The value "M" was replaced with "Married", and the value "S" was replaced with "Single" for the "Marital Status" column. Meanwhile, the value "M" was replaced with "Male", and the value "F" was replaced with "Female" for the "Gender" column.
  - **Nested IF Statements** were used for creating the range columns. The "Income Range" column included three income levels: "Poor", "Middle Class", and "Rich". Any income less than $40,000 was considered "Poor", any income between $40,000 (inclusive) and $100,000 (exclusive) was considered "Middle Class", and any income $100,000+ was considered "Rich". Meanwhile, the "Children Range" column included three levels as well: "No Children", "1-3 Children", and "4-5 Children".

- **Creating Pivot Tables and their Corresponding Graphs**:
  - Refer to the *Pivot Table* worksheet in the Excel workbook
  - **Clustered Bar Charts** were created to help with analyzing how the average income changes across "Gender", "Marital Status", "Occupation", and "Education Level", depending on whether or not a bike is owned. For instance, when taking into account the "Gender" variable, it's shown that both males and females who own bikes have higher incomes on average, with males having a higher income overall on average compared to females. Similarly, those who are married are shown to overall have higher incomes on average compared to those who are single. However, regardless of marital status, it appears that bike owners have higher incomes on average.
  - **Stacked Line Chart** was created to help with analyzing whether the commute distance to work may affect an employee's decision to own a bike. It appears that employees who commute shorter distances to work tend to own more bikes.
  - **Stacked Bar Charts** were created to help with analyzing how the # of bikes vs. cars owned changes based on how many children an employee has and their "Region". Interestingly, employees who have the most children tend to own less of both cars and bikes compared to employees who don't have any children. Similarly, employees who recide in "North America" own a greater number of all vehicles compared to other regions. However, regardless of both "Region" and "Children Range", employees tend to own an equal amount of bikes and cars.

- **Creating Dashboard**:
  - Refer to the *Dashboard* worksheet in the Excel workbook
  - **Slicers** were used to filter out the desired values from the graphs. The slicers corresponding to "Gender", "Marital Status", "Occupation", and "Education" were applied to the clustered bar charts measuring how the average income changes across "Gender", "Marital Status", "Occupation", and "Education Level", depending on whether or not a bike is owned. For instance, married females, regardless of whether or not they own bikes, have higher incomes on average than single females. Meanwhile, the slicers corresponding to "Income Range" and "Children Range" were applied to the stacked bar charts measuring how the # of bikes vs. cars owned changes based on how many children an employee has and their "Region". Although overall employees in North America have more vehicles, employees who are considered poor have more vehicles in Europe. Finally, the slicer corresponding to "Region" was applied to all the graphs.
