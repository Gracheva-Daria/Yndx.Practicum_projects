## 🎯 Цель проекта
Проанализировать базу данных книжного сервиса (при помощи SQL-запросов) и выявить ключевые характеристики и данные, которые помогут сервису для чтения книг сформулировать  ценностное предложение для нового продукта.
<hr>

## 📂 Исходные данные для анализа
**5 таблиц:**

Таблица `books`: содержит данные о книгах.

Таблица `authors`: содержит данные об авторах.

Таблица `publishers`: содержит данные об издательствах.

Таблица `ratings`: содержит данные о пользовательских оценках книг.

Таблица `reviews`: содержит данные о пользовательских обзорах.
<hr>

## ⌛ В ходе выполнения проекта произвела
Коннекцию к базе данных, осмотр содержимого таблиц, написание 5 SQL-запросов. Сформулировала общий вывод по результатам запросов.
<hr>

## 📃 Общий вывод
В результате анализа установлено:
1. Количество книг, вышедших после 1 Января 2000 года: 821 книга.
2. 1) Из ТОП-10 книг по количеству обзоров 9 книг получили по 6 обзоров, и только 1 книга-лидера получила 7 обзоров: "Twilight (Twilight #1)".
   2) Средний рейтинг книг (из ТОП-10 книг по количеству обзоров колеблется) от 3.4 до 4.4 баллов.
3. Издательство, выпустившее наибольшее число книг (книги с более, чем с 50 стр.): "Penguin Books"(42 книги).
    На 2 месте издательство "Vintage" (31 книга) и на 3 месте - "Grand Central Publishing" (25 книг).
4. Автор с самой высокой средней оценкой книг (книги с 50 и более оценками): J.K. Rowling/Mary GrandPré - 4.28 балла.
5. Среднее количество обзоров от пользователей (поставивших более 50 оценок): 24.3.
<hr>

## 🛠️ Используемые инструменты
`Python`, `Pandas`, `SQL`, `SQLAlchemy`
