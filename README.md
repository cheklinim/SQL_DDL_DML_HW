# Домашнее задание к занятию "Работа с данными (DDL/DML)" - Чеклин Иван Михайлович


---

### Задание 1

1. Результат выполнения запроса на получение списка пользователей в базе данных
![users](/img/1.png)

2. Результат выполнения запроса на получение списка прав для пользователя sys_temp
![grants](/img/2.png)`

3. ER-диаграмма получившейся базы данных sakila
![sakila](/img/3.png)`

#### Выполненные скрипты:
```
CREATE USER 'sys_temp'@'localhost' IDENTIFIED BY '12345';
SELECT User FROM mysql.user;
GRANT ALL PRIVILEGES ON *.* TO 'sys_temp'@'localhost';
FLUSH PRIVILEGES;
SHOW GRANTS FOR 'sys_temp'@'localhost';
ALTER USER 'sys_temp'@'localhost' IDENTIFIED WITH mysql_native_password BY '12345';
```

---

### Задание 2

| # | Table name | Primary Key |
| :---: | :---: | :---: |
| 1 | actor	| actor_id |
| 2 | address	| address_id |
| 3 | category	| category_id |
| 4 | city	| city_id |
| 5 | country	| country_id |
| 6 | customer	| customer_id |
| 7 | film	| film_id |
| 8 | film_actor	| actor_id |
| 9 | film_actor	| film_id |
| 10 | film_category	| film_id |
| 11 | film_category	| category_id |
| 12 | film_text	| film_id |
| 13 | inventory	| inventory_id |
| 14 | language	| language_id |
| 15 | payment	| payment_id |
| 16 | rental	| rental_id |
| 17 | staff	| staff_id |
| 18 | store	| store_id |

---
