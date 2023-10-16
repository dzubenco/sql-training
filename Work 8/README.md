<h2 align="center">Work #5</h2>

---

<h2 align="center">Exercises</h2>

* Table `HumanResources.Employee` from `AdventureWorks2019` database contains a field called `LoginID`. It is filled with the data using the pattern [db_name]\\[username] as shown at the screenshot below. Write a query which returns usernames only (data after "\\" symbol) as shown at highlighted part of the screenshot

	![222](https://github.com/dzubenco/sql-training/assets/74211642/d3d993fa-0b9a-46bc-9725-095318a8f08b)

---
* Check the content of `Person.Person`, `Person.PersonPhone` and `Person.PhoneNumberType` tables from  `AdventureWorks2019` database. Write a query that shows each person's First Name, Last Name, Phone Number, but only for the recors with "Employee" Person Type and "Work" Phone Type (please do not "hardcode" the phone type, use subquery or join instead)
---
* **Prerequisite**: run the following query in the `AdventureWorks2019` database connection script:
	
	```
	delete from Person.EmailAddress where BusinessEntityID between 286 and 298;
	```
	
	Then using tables `Person.Person` and `Person.EmailAddress` write a query which will show all the fields from the `Person` table only for the entries which does not have an email set up in `EmailAddress` table.
---
* **Prerequisite**: run the following query in AdventureWorks2019 database :

	```
	Update HumanResources.JobCandidate set BusinessEntityID = 212 where jobCandidateId = 6;
	```
	
	Table `HumanResources.JobCandidate` contains info about candidates. Entries with non-NULL `BusinessEntityID` field already have an interviewer assigned - this `BusinessEntityID` represents interviewer's ID.

	![333](https://github.com/dzubenco/sql-training/assets/74211642/3fcb4446-a872-44d3-87d7-0f1f59c260bf)

	So, using the following tables:

	`HumanResources.JobCandidate`
	`HumanResources.Employee`
	`Person.Person`
	`Person.PersonPhone`
	`Person.PhoneNumberType`

	Write a query which returns info about all currently assigned interviewers in `JobCandidate` table: their `FirstName` and `LastName`, and a `PhoneNumber` if the type of PhoneNumber is "Work"; if it's not "Work" - default Phone Number to '8-800-555-35-35'
	Info about the same interviewer should appear only **ONCE**.

---
* This excercise uses `AdventureWorksLT2019` database, not `AdventureWorks2019` - be careful

	Write a query which will show all Customer FN/LN from table `Customers` and their respective Address ID's from table `CustomerAddress`. In case if there's more than one address for a particluar customer in the `CustomerAddress` table, choose the record with `AddressType` = 'Main Office'. Result dataset should contain only 1 row for each Customer.

	Don't be shy to use subqueries.
