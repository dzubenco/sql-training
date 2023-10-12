<h2 align="center">Work #4</h2>

---

Check out the following videos and answer the questions below:


Group By and Having: [YouTube](https://www.youtube.com/watch?v=oWkvHodS9cA) or [Here](https://raw.githubusercontent.com/dzubenco/sql-training/main/Work%204/Resources/SQL%20Server%20Queries%20Part%2010%20-%20GROUP%20BY%20and%20HAVING.mp4)

Subqueries: [YouTube](https://www.youtube.com/watch?v=5KXbdkv9hEM) or [Here](https://raw.githubusercontent.com/dzubenco/sql-training/main/Work%204/Resources/SQL%20Server%20Queries%20Part%2011%20-%20Subqueries.mp4)

Correlated subqueris: [YouTube](https://www.youtube.com/watch?v=0ETfzlAQqBQ) or [Here](https://raw.githubusercontent.com/dzubenco/sql-training/main/Work%204/Resources/SQL%20Server%20Queries%20Part%2012%20-%20Correlated%20Subqueries.mp4)


---

<h2 align="center">Questions</h2>

<h2 align="left">Group By and Having</h2>

* Which function does not belong to the same group as others? 

    - [ ] MIN()
    - [ ] COUNT()
	- [ ] ROUND()
    - [ ] AVG()

* Look at the query below. Is it a valid one?

	```
	SELECT GroupName, AVG(Mark), COUNT(*)
	FROM Students
	GROUP BY GroupName;
	```

    - [ ] Yes
    - [ ] No
 
* Look at the query below. Is it a valid one?

	```
	SELECT GroupName,  AVG(Mark), COUNT(*)
	FROM Students
	ORDER BY GroupName
	GROUP BY GroupName;
	```

    - [ ] Yes
    - [ ] No
	
* What is the difference between GROUP BY and GROUP BY WITH ROLLUP?

* How behaves GROUP BY WIH ROLLUP if you are grouping by two or more fields?

* What is the difference between WHERE and HAVING clauses?

* Using `Address` and `CustomerAddress` tables from `AdventureWorksLT2019` database, write a query that: Calculates a count of records under  each separate `Address.CountryRegion` and `CustomerAddress.AddressType` fields combination. The query should not return row if the count is greater than 100. It should also take only the records with non-NULL values in `Address.AddressLine2` field. Please provide the whole query as the answer.

<h2 align="left">Subqueries</h2>

* Where subqueries can be used? 

    - [ ] In WHERE filtering criteria
    - [ ] In SELECT
    - [ ] In both SELECT and WHERE
	
* Using `AdventureWorksLT2019` database, write a query that returns all the records from `SalesOrderDetail` table which have `OrderQty` equal to or less than the average value of `OrderQty` from the same table. Please provide the whole query as the answer

* Using `AdventureWorksLT2019` database, write a query that returns all the records from `Address` table which have the same `City` value as the record with `AddressID` = 451. Please provide the whole query as the answer

* In `AdventureWorksLT2019` database, write a script using subqueries which: Takes all the records from `SalesOrderDetail` table with `unitPrice` between 1000 and 2000, and using their `ProductID` returns records for the same `ProductID` but which are for the `unitPrice` < 1000. Please provide the whole query as the answer

<h2 align="left">Correlated Subqueries</h2>

* What is mandatory for correlated subquery? 

    - [ ] Connection with the outer query via the key
    - [ ] Aggregation function usage
	- [ ] Both

* In `AdventureWorksLT2019` database, write a script using subqueries which:

	Returns records with highest `CustomerID` from `Customer` table for each `CompanyName`.

	For example, there are two records `CompanyName` = 'A Great Bicycle Company'
	So, for this compane only record with `CustomerID` = 29872 should be returned.

	Please provide the whole query as the answer
