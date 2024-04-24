* film tablosunda film uzunluğu length sütununda gösterilmektedir. Uzunluğu ortalama film uzunluğundan fazla kaç tane film vardır?

```sql
SELECT * FROM film
WHERE length >
(SELECT AVG(length) from film);
```

* film tablosunda en yüksek rental_rate değerine sahip kaç tane film vardır?

```sql
SELECT COUNT(*) FROM film
WHERE rental_rate = 
(SELECT MAX(rental_rate) FROM film);
```

* film tablosunda en düşük rental_rate ve en düşüK replacement_cost değerlerine sahip filmleri sıralayınız.

```sql
SELECT * FROM film
WHERE rental_rate = 
(SELECT MIN(rental_rate) FROM film)
OR
replacement_cost = 
(SELECT MIN(replacement_cost) FROM film);
```

* payment tablosunda en fazla sayıda alışveriş yapan müşterileri(customer) sıralayınız.

```sql
SELECT first_name,toplam FROM (SELECT customer_id,COUNT(*) AS toplam FROM payment
GROUP BY customer_id) AS total_shopping 
INNER JOIN customer
ON total_shopping.customer_id = customer.customer_id
ORDER BY toplam DESC;
```