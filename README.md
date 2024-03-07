# Committing-and-Rolling-Back-a-Transaction

A transaction is simply a sequence of operations performed using one or more SQL statements as a single logical unit of work. A database transaction must be ACID (Atomic, Consistent, Isolated and Durable). The effects of all the SQL statements in a transaction can either be applied to the database using the COMMIT command or undone from the database using the ROLLBACK command. 

The data used in this lab is internal data. You will be working on the *BankAccounts* and *ShoeShop* tables which are available via 2 DDL scripts.

Scenario: Rose is buying a pair of boots from ShoeShop. So we have to update Rose's balance as well as the ShoeShop balance in the BankAccounts table. Then we also have to update Boots stock in the ShoeShop table. After Boots, let's also attempt to buy Rose a pair of Trainers.
- Once the tables are ready, create a stored procedure routine named TRANSACTION_ROSE that includes TCL commands like COMMIT and ROLLBACK.
- Now develop the routine based on the given scenario to execute a transaction.
- To create the stored procedure routine on MySQL, copy the code below and paste it to the textarea of the SQL page.

Then create a stored procedure TRANSACTION_JAMES to execute a transaction based on the following scenario: First buy James 4 pairs of Trainers from ShoeShop. Update his balance as well as the balance of ShoeShop. Also, update the stock of Trainers at ShoeShop. Then attempt to buy James a pair of Brogues from ShoeShop. If any of the UPDATE statements fail, the whole transaction fails. You will roll back the transaction. Commit the transaction only if the whole transaction is successful.
