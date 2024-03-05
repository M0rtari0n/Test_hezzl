# Test_hezzl

Есть таблица в базе Postgresql
Id (int)
campaignId (int)
playerId (int)
login (string)
date (timestamp)

Напишите SQL запрос в базу, который бы достал все записи с учетом фильтров:
1. campaignId = 145602
2. 31 декабря 2023 <=  date < 31 января 2024

На выходе предоставить пример запроса:

  SELECT * FROM
  
  WHERE campaignId = 145602 AND date >= '2023-12-31' AND date < '2024-01-31';
  
---

Опишите 5-10 тест кейсов на регистрацию пользователя в игре Хезлмания по email

---

Условие:

- Вводим валидные значения в поле email 
   
Шаги:

  1. Зайти на сайт https://play.hezzl.com/
  2. Нажать кнопку "Войти" в правом верхнем углу
  3. Заполнить строку email валидными данными
  4. Нажать кнопку "Войти"
     
Ожидаемый результат:

- Пользователь зарегистрирован, всплывает окно о успешной регистрации.
  
Фактический результат:

- Пользователь зарегистрирован, всплывает окно о успешной регистрации.

---

Условие:

- Поле email не должно быть пустым
  
Шаги:

  1. Зайти на сайт https://play.hezzl.com/
  2. Нажать кнопку "Войти" в правом верхнем углу
  3. Не заполнять строку email
  4. Нажать кнопку "Войти"
     
Ожидаемый результат:

- Пользователь не зарегистрирован, всплывает сообщение, что поле "Email" не может быть пустым.
  
Фактический результат:

- Пользователь не зарегистрирован, всплывает сообщение, что поле "Email" не может быть пустым.

---

Условие:

- Поле email не может содержать пробелы
  
Шаги:

  1. Зайти на сайт https://play.hezzl.com/
  2. Нажать кнопку "Войти" в правом верхнем углу
  3. Заполнить строку email с пробелом
  4. Нажать кнопку "Войти"
     
Ожидаемый результат:

- Пользователь не зарегистрирован, всплывает сообщение, что поле "Email" не может содержать пробелы.
  
Фактический результат:

- Пользователь не зарегистрирован, всплывает сообщение, что поле "Email" не может содержать пробелы.

---

Условие:

- Поле email не регистрозависимое

Шаги:

  1. Зайти на сайт https://play.hezzl.com/
  2. Нажать кнопку "Войти" в правом верхнем углу
  3. Заполнить строку валидными данными с разным регистром.
  4. Нажать кнопку "Войти"
     
Ожидаемый результат: 

- Пользователь зарегистрирован, всплывает окно о успешной регистрации.
  
Фактический результат: 

- Пользователь зарегистрирован, всплывает окно о успешной регистрации.

---

Условие:

- Поле email должно содержать буквы латинского алфавита
  
Шаги:

  1. Зайти на сайт https://play.hezzl.com/
  2. Нажать кнопку "Войти"
  3. Заполнить строку email кириллицей.
  4. Нажать кнопку "Войти"
     
Ожидаемый результат:

- Пользователь не зарегистрирован, всплывает окно о запрещенных символах.
  
Фактический результат:

- Пользователь не зарегистрирован, всплывает окно о запрещенных символах.
