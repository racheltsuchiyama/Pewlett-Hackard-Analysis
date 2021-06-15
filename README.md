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

<img width="742" alt="mentorshipeligibility" src="https://user-images.githubusercontent.com/83552696/121980279-7fc2b580-cd40-11eb-9a7b-6c959f4f660d.png">

With the retiring titles and mentorship elgibility tables, Pewlett Hackward can make an adequately prepare for the large number of employees set to retire.

## Summary

The large wave of retiring employees, called the silver tsunami, would have a large impact on the company. I created a new table that contained the titles of the employees that were elibile for the mentorship program:

<img width="219" alt="me_titlescount" src="https://user-images.githubusercontent.com/83552696/121980336-9bc65700-cd40-11eb-8695-903981cd0bd4.png">

The largest number of employees elibile for the mentorship program were senior staff. These employees could mentor the current staff members in preparation for their retirement. There were also a large number of senior engineers and engineers eligible for the program. Therefore, Pewlett Hackward should focus on hiring new engineers and mentoring them, along with mentoring the current assistant engineers at the company.


Due to the large number of retiring employees, the mentorship eligibilty should be extended to employees born in 1964 and 1965. The number of employees born in 1965 would not be sufficient to supplement the impending silver tsunami. However, including the employees born in 1964 adds thousands of more employees to the program:

<img width="215" alt="Screen Shot 2021-06-14 at 6 52 11 PM" src="https://user-images.githubusercontent.com/83552696/121981011-ce248400-cd41-11eb-8fb7-95baf1140316.png">

