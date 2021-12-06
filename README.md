# Give Me the Goods: More Introductory SQL Queries

## Like

### Wildcards (Regex)
Select all records from the **Students** table where the second letter of the **City** is an "a".

select * from Students where City like '_a%';

*(Add your query to the file exercise1.sql)*


Select all records from the **Students** table where the first letter of the **City** is an "a" or a "c" or an "s".

select * from Students where City like 'a%' or City like 's%' or City like 's%';

*(Add your query to the file exercise2.sql)*


Select all from the **Students** table records where the first letter of the **City** starts with anything from an "a" to an "f".

select * from Students where City between 'a%' and 'f%';

*(Add your query to the file exercise3.sql)*


Select all records from the **Students** table where the first letter of the **City** is NOT an "a" or a "c" or an "f".

select * from Students where City not like 'a%' and City not like 'c%' and City not like 'f%';

*(Add your query to the file exercise4.sql)*


## IN
Use the **IN** operator to select all the records from the **Students** table where **Country** is either "Sint Maarten" or "Haiti".

select * from Students where Country in ('Sint Maarten', 'Haiti');

*(Add your query to the file exercise5.sql)*


Use the **IN** operator to select all the records from the **Students** table where **Country** is NOT "Sint Maarten" and NOT "Haiti".

select * from Student where Country not in ('Sint Maarten', 'Haiti');

*(Add your query to the file exercise6.sql)*
 
## Between values

Use the **BETWEEN** operator to select all the records from the **Courses** table where the value of the **CreditHours** column is between 10 and 20.

select * from Courses where CreditHours between 10 and 20;

*(Add your query to the file exercise7.sql)*

Use the **BETWEEN** operator to select all the records from the **Courses** table where the value of the **CreditHours** column is NOT between 10 and 20.

select * from Courses where CreditHours not between 10 and 20;

*(Add your query to the file exercise8.sql)*

Use the **BETWEEN** operator to select all the records from the **Courses** table where the value of the **CourseName** column is alphabetically between 'ColdFusion' and 'Python'.

select * from Courses where CourseName between 'ColdFusion' and 'Python';

*(Add your query to the file exercise9.sql)*

## Aliases

When displaying the **Students** table, make an alias of the **PostalCode** column, the column should be called **Zip** instead.

select PostalCode as Zip from Students;

*(Add your query to the file exercise10.sql)*


When displaying the **Students** table, refer to the table as **Learners** instead of Students.

select * from Students as Leaners;

*(Add your query to the file exercise11.sql)*
