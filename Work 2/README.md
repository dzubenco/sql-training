<h2 align="center">Work #2</h2>

---

Check out the following videos and answer the questions below:


Calculated columns: [YouTube](https://www.youtube.com/watch?v=JvpFp7E9iFE) or [Here](https://raw.githubusercontent.com/dzubenco/sql-training/main/Work%202/Resources/SQL%20Server%20Queries%20Part%204%20-%20Calculated%20Columns%20in%20Queries.mp4)

Case expressions: [YouTube](https://www.youtube.com/watch?v=zlgrhj2D63E) or [Here](https://raw.githubusercontent.com/dzubenco/sql-training/main/Work%202/Resources/SQL%20Server%20Queries%20Part%205%20-%20CASE%20Expressions.mp4)

JOINs: [YouTube](https://www.youtube.com/watch?v=MJv6ZQlK_ek) or [Here](https://raw.githubusercontent.com/dzubenco/sql-training/main/Work%202/Resources/SQL%20Server%20Queries%20Part%206%20-%20JOINS%20(Inner%20and%20Outer%20Joins).mp4)


---

<h2 align="center">Questions</h2>

<h2 align="left">Calculated columns</h2>

* Can we use aliases of calculated columns in ORDER BY statement?
   * Yes
   * No

* Can we use aliases of calculated columns in WHERE condition? 
   * Yes
   * No
 
* If you want to divide a value of field with Int datatype by any number and get a decimal result, what would be the easiest way to achieve this?
 
* What operator can be used to get a remainder of the division of two numbers?
 
<h2 align="left">Case expressions</h2>

* What type of conditions can be used in WHEN condition of CASE expression?
  * >, <, >=, <=, <>
  * Any condition that returns boolean value - true or false
 
* What is the syntax for default option in CASE expression?
  * DEFAULT
  * ELSE
 
* Can alias of CASE expression be used in WHERE statement? If not, why? 

<h2 align="left">JOINs</h2>

* What is not necessary if you are going to join two tables using INNER JOIN statement? 
  * Join matching condition
  * To give aliases to the table(s)
 
* If you put "*" in the SELECT criteria of a query which contains INNER JOIN of two tables, what will the result contain? 
  * Fields of the left table
  * Fields of the right table
  * Fields of the both tables
  * Fields mentiond in the join matching condition

* Outer joins are mostly used for ...

* Imagine that we are running a query. What do we need to add to this query in order to get only account names for the accounts which present in table A but do not present in table B?

```
SELECT A.AccountName
FROM A
LEFT OUTER JOIN B
ON A. AccountID = B. AccountID ;
```

* Does it matter in that order the table names are listed around INNER JOIN statement?
  * Yes
  * No

* Can you use LEFT JOIN instead of LEFT OUTER JOIN?
  * Yes
  * No

* How can you change a query with LEFT OUTER JOIN statement to return the same data but not using LEFT OUTER JOIN?

* The Join Matching condition should always contain at least one field of one of the tables
  * True
  * False
