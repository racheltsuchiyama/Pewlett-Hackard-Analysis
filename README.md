# Pewlett-Hackard-Analysis

## Purpose

The purpose of this project was to analyse the employee data from the company Pewlett Hackard. Many of the employees were nearing retirement age, so I determined how many of the employees were set to retire. Then, I found the job titles of those retiring employees to determine which positions would need to be filled. Pewlett Hackward wanted to start a mentorship program between the retiring employees and new hires to ensure a smooth transition. Therefore, I created a new table to store all the employees eligible for the mentorship program.

### Data and Software
Using the data from the employees.csv, departments.csv, titles.csv, salaries.csv, dept_emp.csv, and dept_manager.csv, queried on pgAdmin 4.

## Results 

* **Retirement Titles**
First, I wanted to find all the employees that were retiring and their job titles. I combined the employees.csv and titles.csv to create a new table with the desired information for employees born between 1952 and 1955.

<img width="659" alt="retirement_titles" src="https://user-images.githubusercontent.com/83552696/121820417-786bb100-cc47-11eb-9092-a74ce0810df4.png">

The retirement titles table contained all the titles that the employees held. While it was useful to have a comprehensive list of the retiring employees, the previous titles held by these employees was not relevent to the mentorship program.

* **Unique Titles**

By filtering the retirement titles table, I created a new table containing only the most recent titles of the retiring employees: 

<img width="486" alt="unique_titles" src="https://user-images.githubusercontent.com/83552696/121820422-7f92bf00-cc47-11eb-83ee-5b641caf9558.png">

This table provided the company with a list of the roles that would need to be filled whent these employees retire.

* **Retiring Titles**

To see how many employees are retiring from each department, I created a new table by extracting the counts of the titles from the unique titles table.

<img width="222" alt="retiring_titles" src="https://user-images.githubusercontent.com/83552696/121820427-87eafa00-cc47-11eb-9bef-bec4d02aa807.png">

Most of the retiring employees were either senior engineer or senior staff members. Therefore, the employees Pewlett Hackard should hire should primarily be engineers.

* **Mentorship Elgibility**

The employees eligible to participate in the mentorship program were the closet to retiring. Therefore, I extracted all the current employees born in 1965.



With the retiring titles and mentorship elgibility tables, Pewlett Hackward can make an adequately prepare for the large number of employees set to retire.

## Summary



Provide high-level responses to the following questions, then provide two additional queries or tables that may provide more insight into the upcoming "silver tsunami."

How many roles will need to be filled as the "silver tsunami" begins to make an impact?

Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
