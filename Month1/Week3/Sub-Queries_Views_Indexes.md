# Optimize Your SQL Queries with Subqueries, Views, and Indexes in SSMS.

Subqueries are queries that are `embedded` within another query. They can be used to `retrieve data` that will be used in the `main query,` or to `filter` or `aggregate` data before it's returned. There are `four types` of subqueries: 

- single-row, 
- multi-row,
- nested, and 
- correlated. 

Let's go through each one in turn.


## Single-Row Subqueries:
A `single-row subquery` is a query that `returns only one row` of data. It's often used as a `filter to restrict` the results of the `main query.`
## Here's an example:
```sql
SELECT *
FROM employees
WHERE salary > (SELECT AVG(salary) FROM employees);
```
In this example, the subquery calculates the average salary of all employees, and the main query returns only those employees whose salary is greater than the average.

## Multi-Row Subqueries:
A multi-row subquery is a query that `returns more than one row` of data. It's often used as a `filter` or to provide data for an `IN clause.`
## Here's an example:
```sql
SELECT *
FROM employees
WHERE department_id IN (SELECT department_id FROM departments WHERE location = 'New York');
```
In this example, the subquery returns all department IDs for departments located in New York, and the main query returns all employees who work in those departments.

## Nested Subqueries:
A nested subquery is a query that `contains another subquery.` It's often used to perform `complex filtering` or `aggregation.`
## Here's an example:
```sql
SELECT *
FROM employees
WHERE department_id IN (SELECT department_id
FROM departments
WHERE location = (SELECT location FROM locations WHERE city = 'San Francisco'));
```
In this example, the nested subquery retrieves the location of San Francisco from the locations table, the inner subquery returns all department IDs for departments located in San Francisco, and the main query returns all employees who work in those departments.

## Correlated Subqueries:
A correlated subquery is a query that uses a `value` from the `outer query` in the `subquery.` It's often used to `filter data` based on a `condition` in the `outer query.`
## Here's an example:
```sql
SELECT *
FROM employees e
WHERE salary > (SELECT AVG(salary) FROM employees WHERE department_id = e.department_id);
```
In this example, the correlated subquery calculates the average salary for employees in the same department as the employee in the outer query, and the main query returns only those employees whose salary is greater than the department average.
