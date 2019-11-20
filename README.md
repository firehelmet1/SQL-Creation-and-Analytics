# SQL Analysis of an Employee Database: A Mystery in Two Parts

![sql.png](sql.png)

## Background

In this project, I designed the SQL database tables to hold employee data in the sCSVs, imported the CSVs into a SQLite database, and analyzed the data:

1. Data Modeling

2. Data Engineering

3. Data Analysis


#### Data Modeling

Inspect the CSVs and sketch out an ERD of the tables. The following tool is helpful in architecting the database [http://www.quickdatabasediagrams.com](http://www.quickdatabasediagrams.com).

(employees_db_quickdbd.JPG)

#### Data Engineering

* Create a table schema for each of the six CSV files specifying data types, primary keys, foreign keys, and other constraints.


#### Data Analysis

Inside the SQL database, the following analysis was performed.

1. List the following details of each employee: employee number, last name, first name, gender, and salary.

2. List employees who were hired in 1986.

3. List the manager of each department with the following information: department number, department name, the manager's employee number, last name, first name, and start and end employment dates.

4. List the department of each employee with the following information: employee number, last name, first name, and department name.

5. List all employees whose first name is "Hercules" and last names begin with "B."

6. List all employees in the Sales department, including their employee number, last name, first name, and department name.

7. List all employees in the Sales and Development departments, including their employee number, last name, first name, and department name.

8. In descending order, list the frequency count of employee last names, i.e., how many employees share each last name.


Visualization analysis of the average salary by title indicates a several strange discrepancies in compensation:
•	Sr. Engineer / Engineer / Assistant Engineer have equivalent salaries (Sr Engineer should be notably higher than Engineer, notably higher than Assistant Engineer)
•	Staff & Sr. Staff have equivalent salaries (Sr. Staff should be notably higher)
•	Managers are less compensated lower than Staff / Sr. Staff (generally not the case)
•	Technique Leader appears to be the lowest paid (generally they are among the highest paid).

 (salarytitle.png)

The maximum salaries also show similar discrepancies
•	Maximum salary for a manager is the lowest (even lower than an assistant engineer)
•	Staff & Sr. Staff again show equivalent maximums
•	Sr. Engineer and Engineer show equivalent maximums
 
(maxsalarytitle.png)
