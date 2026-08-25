# shekha.chand14
SQL Basics

SELECT customer_name, country FROM customers;
SELECT DISTINCT country FROM customers;
SELECT COUNT(DISTINCT country) FROM customers;

SELECT * FROM customers
WHERE city = 'London';

SELECT * FROM products
ORDER BY price;

SELECT * FROM products
ORDER BY price DESC;

SELECT * FROM customers
LIMIT 20;

SELECT * FROM customers
LIMIT 20 OFFSET 40;

SELECT MIN(price)
FROM products;

SELECT MAX(price)
FROM products;

SELECT MIN(price) AS lowest_price
FROM products;

SELECT COUNT(customer_id)
FROM customers;

SELECT COUNT(customer_id)
FROM customers
WHERE city = 'London';

SELECT SUM(quantity)
FROM order_details;

SELECT AVG(price)
FROM products;

SELECT AVG(price)::NUMERIC(10,2)
FROM products;

SELECT * FROM customers
WHERE customer_name LIKE 'A%';

SELECT * FROM customers
WHERE customer_name LIKE '%A%';

SELECT * FROM customers
WHERE customer_name ILIKE '%A%';

SELECT * FROM customers
WHERE customer_name LIKE '%en';
	
SELECT * FROM customers
WHERE city LIKE 'L_nd__';

SELECT * FROM customers
WHERE country IN ('Germany', 'France', 'UK');

SELECT * FROM customers
WHERE country NOT IN ('Germany', 'France', 'UK');

SELECT * FROM customers
WHERE customer_id IN (SELECT customer_id FROM orders);

SELECT * FROM customers
WHERE customer_id NOT IN (SELECT customer_id FROM orders);

SELECT * FROM Products
WHERE Price BETWEEN 10 AND 15;

SELECT * FROM Products
WHERE product_name BETWEEN 'Pavlova' AND 'Tofu';

SELECT * FROM orders
WHERE order_date BETWEEN '2023-04-12' AND '2023-05-05';

SELECT customer_id AS id
FROM customers;

SELECT customer_id id
FROM customers;

SELECT product_name || unit AS product
FROM products;

SELECT product_name AS "My Great Products"
FROM products;














