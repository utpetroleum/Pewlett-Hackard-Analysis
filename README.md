# Pewlett-Hackard-Analysis

## Overview of Project

### Purpose
The purpose of this project is to determine the number of retiring employees per title and identify employees who are eligible to participate in a mentorship program. Then, in a report summarizes the analysis and helps prepare the manager for the “silver tsunami” as many current employees reach retirement age. 

## Results

### The Number of Retiring Employees by Title

retiring_titles table:

![Retiring Employees by Title](https://user-images.githubusercontent.com/92401000/144724937-0accc64b-7943-4f06-adc9-79d9caf785bb.PNG)

- The greatest number of employees retiring will be from "Senior Engineer" and "Senior Staff". 29,414 "Senior Engineer" and 28,254 "Senior Staff" is of retirement age.

- The least number of employees retiring will be from "Assistant Engineer" and "Manager". 1,761 "Assistant Engineer" and 2 "Manager" is of retirement age. 

### The Employees Eligible for the Mentorship Program

mentorship_count sum query:

![Employees Eligible for the Mentorship Program](https://user-images.githubusercontent.com/92401000/144724942-ca8c1e78-758d-43df-9305-87bcb86b6d81.PNG)

- Throughout the entire company of Pewlett Hackard, only 1,549 current employees are eligible to participate in a mentorship program. 

- There are zero employees under the "Manager" title eligible to participate in a mentorship program. 

## Summary

### How many roles will need to be filled as the "silver tsunami" begins to make an impact?

retiring_titles sum query:

![retiring_titles sum](https://user-images.githubusercontent.com/92401000/144730381-082aea6b-dae6-43e0-ae50-c2a34fe30757.PNG)

Using the sum function on retiring_titles table, we find that there will be a total of 90,398 retiring soon so we would need 90,398 new employees to make up for those retiring.

### Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?

mentorship_count table:

![Employees Eligible for the Mentorship Program](https://user-images.githubusercontent.com/92401000/144730402-92af6dc4-e9e5-417d-b688-15093f1553e4.PNG)

mentorship_count sum query:

![mentorship_count sum](https://user-images.githubusercontent.com/92401000/144730408-3b9f1309-145d-4b28-8570-eac6e5451e68.PNG)

By creating a new table called "mentorship_count" to count the titles in "mentorship_eligibility" table then performing a query to take the sum of the "mentorship_count" table, we got a sum of 1,549 employees who are mentorship ready. We can conclude that there are not enough qualified, retirement-ready employees who can mentor the new employees who are expected to take the place of 90,398 employees retiring.
