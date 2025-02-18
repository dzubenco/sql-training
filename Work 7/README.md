<h2 align="center">Work #7</h2>

---

Check out the following videos and answer the questions below:

Variables: [YouTube](https://www.youtube.com/watch?v=NmYaOlcbfZM) or [Here](https://github.com/dzubenco/sql-training/raw/refs/heads/main/Work%207/Resources/SQL%20Server%20Programming%20Part%203%20-%20Variables.mp4)

Output Parameters & Return Values: [YouTube](https://www.youtube.com/watch?v=GvRv4V-AK70) or [Here](https://github.com/dzubenco/sql-training/raw/refs/heads/main/Work%207/Resources/SQL%20Server%20Programming%20Part%204%20-%20Output%20Parameters%20&%20Return%20Values.mp4)

---

<h2 align="center">Questions</h2>

* The query below returns top 4 records from table `Employee` (`AdventureWorks2019` database)
  
	```
	SELECT TOP 4 *
	FROM HumanResources.Employee;
	```

	Please add a parameter `@Num` which can be used instead of hardcoded value and check that the query works in a database. Hint: most probably just raplacing `4` with `@Num` will not work.

	Please provide the whole query as the answer.

---
* Can we use a subquery in order to assign an initial value to the variable just in DECLARE statement? Please check in DB
  
	- [ ] Yes
	- [ ] No
---
* What function can be used in case if you want to show some text output in the "Messages" tab of the script output window?
---
* How can you suppress the default message about how much rows have been affected by the query in the "Messages" tab of the script output window?

  ![img1](https://github.com/user-attachments/assets/2a492aca-141a-46ff-a784-01272ea4f777)


---
* Look at the query and it's output at the screenshot below.

	How do you think, what will happen if we'll try to assign the output of this query to a single variable of type int as in the script below?

	```
	DECLARE @test AS INT
	
	SELECT TOP 3 @test = BusinessEntityID
	FROM HumanResources.Employee
	ORDER BY BusinessEntityID DESC
 	```

 	![Img2](https://github.com/user-attachments/assets/63309331-872b-41c3-a0f4-b24b383c998e)

	- [ ] Error appears - the script is invalid to be run
	- [ ] It will assign the value 290 to the variable
	- [ ] It will assign the value 288 to the variable

---
* At the previous work #6 we've created a Stored Procedure which returns some select output - you can double check it [here](https://github.com/dzubenco/sql-training/tree/main/Work%206)

	Now, please create a new one proc which actually soes the same but in another format:
	
	- takes as a parameter `@countNumber`;
	
	- returns you as output parameter the set of ProductId values in a single concatenated string - values should be separated by comma for the products that appear in `ProductListPriceHistory` table `@countNumber` times
	
	- returns you as output parameter the number of rows affected
	
	These two output parameters must be accessable outside of SP after it's invocation
	
	Please see the example at the screenshot below:

	![Img3](https://github.com/user-attachments/assets/eb365515-4057-4281-a567-28ea398dc56b)
