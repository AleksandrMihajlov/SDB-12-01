# SDB-12-01
Базы данных - Aleksandr Mihajlov SYS34  
  
**Задание 1**  
  
Опишите не менее семи таблиц, из которых состоит база данных:

- какие данные хранятся в этих таблицах;  
- какой тип данных у столбцов в этих таблицах, если данные хранятся в PostgreSQL.  

Приведите решение к следующему виду:  
  
Сотрудники (  
  
- идентификатор, первичный ключ, serial,  
- фамилия varchar(50),  
- ...  
- идентификатор структурного подразделения, внешний ключ, integer).

Ответ:  
---  
Сотрудники ( 
- Идентификатор, первичный ключ, serial
- Фамилия, varchar(50), not null  
- Имя, varchar(50), not null
- Отчество, varchar(50)
- Оклад, внешний ключ
- Должность, внешний ключ
- Тип подразделения, внешний ключ
- Структурное подразделение, внешний ключ
- Дата найма, date, not null
- Адрес филиала, внешний ключ
- Проект на который назначен, внешний ключ)  
  
Оклад (  
- Идентификатор, первичный ключ, not null, integer
- Оклад, not null)  
  
Должность (
- Идентификатор, первичный ключ, not null, integer
- Должность, not null, varchar(100))  
  
Тип подразделения (
- Идентификатор, первичный ключ, not null, integer
- Тип подразделения, not null, varchar(50))  
  
Структурное подразделение (
- Идентификатор, первичный ключ, not null, integer
- Структурное подразделение, not null, varchar(100))  
  
Адрес филиала (
- Идентификатор, первичный ключ, not null, integer
- Адрес филиала, not null, varchar(100))  
  
Проект на который назначен (
- Идентификатор, первичный ключ, not null, integer
- Проект на который назначен, not null, varchar(100))