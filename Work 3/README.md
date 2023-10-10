<h2 align="center">Work #3</h2>

---

Check out the following videos and answer the questions below:


Using functions in queries: [YouTube](https://www.youtube.com/watch?v=Fm8od9L9HMg) or [Here](https://raw.githubusercontent.com/dzubenco/sql-training/main/Work%203/Resources/SQL%20Server%20Queries%20Part%207%20-%20Using%20Functions%20in%20Queries.mp4)

Text calculations: [YouTube](https://www.youtube.com/watch?v=HJKraiIoYPU) or [Here](https://raw.githubusercontent.com/dzubenco/sql-training/main/Work%203/Resources/SQL%20Server%20Queries%20Part%208%20-%20Text%20Calculations.mp4)

Date Calculations: [YouTube](https://www.youtube.com/watch?v=Q2xhAafpRJo) or [Here](https://raw.githubusercontent.com/dzubenco/sql-training/main/Work%203/Resources/SQL%20Server%20Queries%20Part%209%20-%20Date%20Calculations.mp4)


---

<h2 align="center">Questions</h2>

<h2 align="left">Functions in queries</h2>

* Each and every function in MS SQL requires at least 1 parameter
    - [ ] True
    - [ ] False

* What will be the correct version of get current date function call? 
    - [ ] SELECT GETDATE()
    - [ ] SELECT GETDATE
 
* Can a result of one function be used as a parameter of another function?
    - [ ] Yes
    - [ ] No

<h2 align="left">Text calculations</h2>

* What is (are) the correct syntax of concatenate function in MS SQL? 
    - [ ] ||
    - [ ] \+
    - [ ] CONCAT()
 
* Do CAST() and CONVERT() functions behave similarly in MS SQL?
    - [ ] Yes
    - [ ] No
 
* You have a table below. Using substring() function instead of right() and left(), write a SQL query which will show the First Name and Last Name only in single field. As an answer please provide a complete SQL query (without any additional text). So in our case, expected output is: [Tom Cruise, Dwayne Johnson]

```
SELECT ActorName
FROM (
	SELECT 'Tom BigBoy Cruise' as ActorName
	UNION
	SELECT 'Dwayne Rock Johnson' as ActorName
) A;
```

<h2 align="left">Date Calculations</h2>

* Try it yourself in DB and answer: what will happen if you will wrongly specify less number of chars than required by date mask? (See example below - when 103 date style requires 10 symbols)
	```
	convert(char(8), SomeDateField, 103)
	```
    - [ ] 2008-06-01 00:00:00.000 --- >  01/06/08
    - [ ] 2008-06-01 00:00:00.000 --- >  01/06/20


  
* Try it yourself in DB and answer: what will happen if you will specify more number of chars than required by date mask? (See example below - when 3 date style requires 8 symbols)
	```
	convert(char(10), SomeDateField, 3)
	```

  
* Write a query to select a month from the RegistryDate field

* Considering that we have the following field with a single row:
	```
	select CAST('2024-09-26 00:00:00.000' AS DATETIME) as FutureModifiedDate
	```
	What will be the output of the following function call?
	```
	DATEDIFF(YY, FutureModifiedDate, GETDATE())
	```
