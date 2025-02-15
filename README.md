# BD
1) Выберите из таблицы orders все заказы

SELECT * FROM orders 

![image](https://github.com/user-attachments/assets/46efc6ca-f163-4f31-9287-5be6a141a4ce)


2) Выберите из таблицы orders все заказы кроме новых. У новых заказов status равен "new". Использовать in

SELECT * FROM orders WHERE STATUS IN ('cancelled','in_progress','delivery')

![image](https://github.com/user-attachments/assets/73c92258-7a54-4388-b66b-5fd97b2017fd)


3) Выберите из таблицы orders все новые и отмененные заказы. У отмененных заказов status равен "cancelled". У новых заказов status равен "new".

SELECT * FROM orders WHERE status IN ('new', 'cancelled');

![image](https://github.com/user-attachments/assets/5fddf410-be1d-4cff-b8ad-6fbfc0d97791)


4) Выберите из таблицы orders все заказы содержащие более 3 товаров (products_count).
Вывести нужно только номер (id) и сумму (sum) заказа.

SELECT id, sum FROM orders WHERE products_count > 3;

![image](https://github.com/user-attachments/assets/10bcca88-bb6c-45b6-9549-c2204f08ec12)

