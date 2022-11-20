# SQL-7
### Perform the following query scenarios on the DVD rental sample database.
1) Group the films in the film table according to their rating values.
2) When we group the films in the film table according to the replacement_cost column, list the replacement_cost value with more than 50 films and the corresponding number of films.
3) customer tablosunda bulunan store_id değerlerine karşılık gelen müşteri sayılarını nelerdir?
4) city tablosunda bulunan şehir verilerini country_id sütununa göre gruplandırdıktan sonra en fazla şehir sayısı barındıran country_id bilgisini ve şehir sayısını paylaşınız.
## Ans
1) SELECT rating FROM film GROUP BY rating;
2) SELECT replacement_cost,COUNT(*) FROM film GROUP BY replacement_cost HAVING COUNT(*)>50;
3) SELECT store_id, COUNT(*) FROM customer GROUP BY store_id;
4) SELECT country_id, COUNT(*) FROM city GROUP BY country_id ORDER BY COUNT(*) DESC LIMIT 1;
