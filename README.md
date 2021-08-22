# Pewlett Hackard Analysis
## Overview
The purpose of this analysis is to help the company Pewlett Hackard determine the number people who are eligible for retirement so they can determinen who is retiring and prepare for the number of future job vacancies. 

## Results
### List of Retiring Employees by Title
A Retirement Titles table was created (retirement_titles.csv) which contains a list of all the titles of the employees who were born between January 1, 1952 and December 31, 1955. 
(image)
However, employees have had multiple titles during their employment with Pewlett Hackard, so there are duplicates of employees. Therefore, we need a table that will keep only the most recent title of each employee. Using the DISTINCT ON function, we are able to create a table that contains the list of retiring employees with only their most recent title (retiring_titles.csv).
(image)

### Number of Retiring Employees by Title
Using the COUNT and GROUP BY functions and selecting the unique_title.csv table, we are able to determine the number of employees retiring grouped by title. This helps give a visual to how many employees from each title are retiring. 
(image)

### List of Employees Eligible for Mentorship Program
Pewlett Hackard wants to know who is eligible to help mentor new employees as a large amount of employees are retiring in the near future. Employees who are born between January 1, 1965 and December 31, 1965 are eligible for the mentorship program. Therefore, a table was created with a list of employees born between those two dates (mentorship_eligibility.csv). 
(image)

### Number of Employees Eligible for Mentorship Program by Title
A list of employees eligible is useful, but it would also be helpful to know the number of employees eligible for the mentorship program by title. Similar to the retiring_titles.csv table, using the COUNT and GROUP BY functions and selecting the mentorship_eligibility.csv, we are able to determine the number of eligible employees grouped by title. This helps give a visual to how many employees are eligible from each title.
(image)

## Summary
There is a very large number of Pewlett Hackard employees, born between January, 1, 1952 and December 31, 1955, who are eligible for retirement. The total number of retirement eligible employees is **90,398**. Therefore, Pewlett Hackard is going to have to fill **90,398** positions as the "silver tsunami" starts to make an impact.

The total number of qualified, retirement-ready employees (born between January 1, 1965 and December 31, 1965) **1,549**. This number is significantly less compared to the number of retiring employees **90,398**. This would require 1 employee to mentor about 57 new employees, and that is not an ideal situation for a mentorship program. Therefore, a new table is created to expand the number of eligible employees for the mentorship by expanding the birth date requirement (born between January 1, 1964 and December 31, 1965). The new table is called mentorship_eligibility_2.csv and it contains the list of employees who were both between January 1, 1964 and December 31, 1965. 
(image)
Also, a table containing the number of eligible employees for the mentorship program grouped by title was also create (mentorship_titles_2.csv).
(image)
With this list of mentorship eligible employees, the number of new employees per mentor employee is a maximum of 4, which is much more manageable. 
