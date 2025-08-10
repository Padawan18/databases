
## Задание 1.
Задание 1
Одним запросом получите информацию о магазине, в котором обслуживается более 300 покупателей, и выведите в результат следующую информацию:

- фамилия и имя сотрудника из этого магазина;

- город нахождения магазина;

- количество пользователей, закреплённых в этом магазине.

```
select  store.store_id, concat(staff.first_name, ' ', staff.last_name) as fio, city,  COUNT(customer.customer_id) from store
JOIN 
    staff ON store.manager_staff_id = staff.staff_id
JOIN 
    customer ON store.store_id = customer.store_id
JOIN 
   city on staff.address_id=city.city_id
GROUP BY 
    store.store_id, fio
HAVING 
    COUNT(customer.customer_id) > 300;
```
Результат 

![test](https://github.com/Padawan18/databases/blob/main/1.png)
