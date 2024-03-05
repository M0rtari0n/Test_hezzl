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

На выходе предоставить пример запроса

SELECT * FROM
WHERE campaignId = 145602 AND date >= '2023-12-31' AND date < '2024-01-31';

Опишите 5-10 тест кейсов на регистрацию пользователя в игре Хезлмания по email

---
