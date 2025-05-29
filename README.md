# DailyCostTracker
DailyCostTracker - for home budgets

The purpose of this application is to help manage my cash flow.  

I can download a list of transactions for my account using my banks web site. The format of the file is a comma separated value file.  
The Daily Cost Tracker understands the format of the file. The first line represents the field header.
The second to n lines represents the transactions.  The tranactions are imported into a local SQL Server Express Database. 

Once the transactions are in the database, it looks at the transactions that do not have a cost or savings category. 
For these transactions, it looks at the description of the transaction and then determines if its an actual cost or a withdrawal that goes into a savings account.

This importer can handle transactions that have already been imported.
