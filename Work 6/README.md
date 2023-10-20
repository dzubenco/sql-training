<h2 align="center">Work #6</h2>

---

Check out the following videos and answer the questions below:


SP Basics: [YouTube](https://www.youtube.com/watch?v=fjNsRV4zLdc) or [Here]()

SP with parameters: [YouTube](https://www.youtube.com/watch?v=Vs-atxMs4mw) or [Here]()

---

<h2 align="center">Questions</h2>

* What is obligatory for a SP creation? 

    - [ ] BEGIN and END reserved words
    - [ ] Mark a batch start with GO reserved word
	- [ ] Provide a name to the SP

---	
* What is the correct syntax to execute getFirstName procedure?

    - [ ] SELECT getFirstName
    - [ ] EXECUTE getFirstName
	- [ ] RUN getFirstName

---	
* What should be used in case is you want to change the code of SP? 

---	
* What should be used in case is you want to delete the SP? 

---
* Assuming that you have the following procedure (you can try to create it in `AdventuryWorks2019` database):

	```
	CREATE PROC getProduct AS
	SELECT *
	FROM Production.Product
	WHERE SafetyStockLevel >= 100;
	```

	Modify it: is should receive as a perameter the min value of `SafetyStockLevel` (instead of hardcoding it to 100)

	Please provide the whole SQL query as an answer
	
---
* Considering that `@Name` - is a parameter of any SP, what is the correct way to apply this parameter to any hardcoded string? 

    - [ ] '@Name is a student'
    - [ ] @Name + ' is a student'
	
---
* What should you use if you need to specify a default value for any of SP parameter? 

---
* Check the content of `Production.ProductListPriceHistory` and `Production.Product` tables from `AdventureWorks2019` database.

	Write a SP that:
	takes as a parameter `@countNumber`;
	returns all the `ProductID`s, `productName`s, `count` of occurencies and maximum value of `ListPrice` for all the products that appear in `ProductListPriceHistory` table `@countNumber` times.

	Please provide the whole SQL query as an answer
