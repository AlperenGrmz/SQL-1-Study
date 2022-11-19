# SQL-2
### Perform the following query scenarios on the DVD rental sample database.
1) Sort the data in all the columns in the film table in the order that the replacement cost value is greater than 12.99, equal to and less than 16.99 ( BETWEEN - AND configuration uses.)
2) Sort the data in the first_name and last_name columns in the actor table provided that first_name is 'Penelope' or 'Nick' or 'Ed'. (Use the IN operator.)
3) Sort the data in all columns in the film table with rental_rate 0.99, 2.99, 4.99 AND replacement_cost 12.99, 15.99, 28.99. (Use the IN operator.)
## Ans
1) SELECT * FROM film WHERE replacement_cost BETWEEN 12.99 AND 16.98;
2) SELECT first_name,last_name FROM actor WHERE first_name IN ('Penelope','Nick','Ed');
3) SELECT * FROM film WHERE rental_rate IN(2.99,0.99,4,99) AND replacement_cost IN(12.99,15.99,28.99);
