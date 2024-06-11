# Сурмач Андрей Андреевич
# SQL-1

# Задание_1

```
SELECT
	DISTINCT district
FROM
	address
WHERE
	LEFT(district, 1) = 'K'
	AND RIGHT(district, 1) = 'a'
	AND POSITION(" " IN district) = 0;
 ```

 [1](https://github.com/Aid1986/SQL-1/blob/main/1.png

 # Задание_2
```
 SELECT
	*
FROM
	payment
WHERE
	amount > 10
	AND payment_date >= '2005-06-15'
	AND payment_date < '2005-06-19';
```
 [2](https://github.com/Aid1986/SQL-1/blob/main/2.png

 # Задание_3
```
 SELECT
	*
FROM
	rental
ORDER BY
	rental_date DESC
LIMIT 5;
```
[3](https://github.com/Aid1986/SQL-1/blob/main/3.png

# Задание_4
```
SELECT
	customer_id,
	store_id,
	REPLACE(LOWER(first_name), 'll', 'pp') AS first_name,
	LOWER(last_name) AS last_name,
	email,
	address_id,
	active,
	create_date,
	last_update
FROM
	customer
WHERE
	active = 1
	AND first_name IN ('Kelly', 'Willie');
```
 [4](https://github.com/Aid1986/SQL-1/blob/main/4.png
