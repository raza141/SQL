# SQL
This repo is all about SQL and using Database MySQL for creating Database to store financial data

### SQL:

- Each Row data is called **Record.**
- Collection of multiple tables in one database called **Schema.**
- We use the semicolon ; in SQL language.
--------------------------------------------------------------------

1. CREATE DATABASE PSX (PSX is the name of database).
2. CREATE TABLE BOP (BOP is the name of table inside the PSX database).

    2.1 *CREATE* TABLE BOP (Date DATE, Open FLOAT, High FLOAT, Low FLOAT, Close FLOAT, Volume INT);
3. ALTER TABLE BOP ADD Pct_Change; (Alter commad is used to add or drop the column from TABLE) here we add the column name Pct_Change
4. **ALTER** TABLE BOP DROP Adj Close; (This will drop the Adj Close column)
5. DROP TABLE BOP (This command will drop the whole Table )
6. **DROP** DATABASE FinancData (This will delet the whole database)
7. **INSERT** INTO BOP (Date,Open, High, Low, Volume) VALUE ('1-1-2023', 3.56,3.64,3.54,3.62); - (Insert command is used to insert the value into table)
8. SELECT * FROM BOP (SELECT : is used to specify the column, * : is used to get the all columns, FROM: to specify the name of TABLE)
9. SELECT Close FROM BOP;  (This will return the Close values from BOP TABLE) 
10. SELECT Close, Volume FROM BOP **ORDER BY** Volume; (This will return the two colmns close and volumes and volumns is ordered)
11. **UPDATE** BOP SET Volume = 100 WHERE Date='1-1-2023' (Update / change the record of volume)
12. **DELETE** FROM BOP WHERE Date= '1-1-2023' ( Delete the record of the date)
13. SELECT **COUNT(*)** FROM BOP; (this is provides the total number Rows in TABLE)
14. **SELECT** Date, Open, Close **FROM** BOP;
15. **WHERE** clause is used to Select the ROW.

    15. 1 SELECT * FROM BOP WHERE Volume > 10,000 AND Date >= '1-1-2022' **ORDER**  BY Volume **DESC** **LIMIT** 1; (Select the Volume greater than and 10,000 and after 1-1-2022 and volume is sorted by Descenting order, this Limit will only display 1 record and improve the speed). 


16. SELECT **DISTINCT** Close FROM BOP; (Distinct function is used to show only unique record not duplicate values)

