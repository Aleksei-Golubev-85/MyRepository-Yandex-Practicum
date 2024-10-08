# Финальный спринт

Финальный спринт включает в себя работу над проектом и задачи по SQL


## Название проекта: Анализ оттока клиентов Метанпромбанка


### Данные

В нашем распоряжении файл **bank_scrooge.csv** - датасет с данными о клиентах банка «Метанпром».  

Структура **bank_scrooge.csv:**

- ***userid***- идентификатор пользователя;
- ***score*** - баллы кредитного скоринга;
- ***city*** - город;
- ***gender*** - пол;
- ***age*** - возраст;
- ***equity*** - количество баллов собственности;
- ***balance*** - баланс на счёте;
- ***products*** - количество продуктов, которыми пользуется клиент;
- ***credit_card*** - есть ли кредитная карта;
- ***last_activity*** - активный клиент;
- ***est_salary*** - оценочный доход клиента;
- ***сhurn*** - признак оттока (целевая переменная).

### Задача

Проанализировать клиентов регионального банка и выделить сегменты клиентов, которые склонны уходить из банка. Дать рекомендации по работе с данными сегментами.

### Используемые библиотеки

*pandas*  
*seaborn*  
*matplotlib*  
*scipy*  
*numpy*  
*math*  
*phik*  
*functools*  

## Проект SQL: Анализ баз данных сервиса для чтения книг по подписке¶

### Данные

Таблица **books** - содержит данные о книгах:

- ***book_id*** — идентификатор книги;
- ***author_id*** — идентификатор автора;
- ***title*** — название книги;
- ***num_pages*** — количество страниц;
- ***publication_date*** — дата публикации книги;
- ***publisher_id*** — идентификатор издателя.

Таблица **authors** - содержит данные об авторах:

- ***author_id*** — идентификатор автора;
- ***author*** — имя автора.

Таблица **publishers** - содержит данные об издательствах:

- ***publisher_id*** — идентификатор издательства;
- ***publisher*** — название издательства.

Таблица **ratings** - содержит данные о пользовательских оценках книг:

- ***rating_id*** — идентификатор оценки;
- ***book_id*** — идентификатор книги;
- ***username*** — имя пользователя, оставившего оценку;
- ***rating*** — оценка книги.

Таблица **reviews** - содержит данные о пользовательских обзорах на книги:

- ***review_id*** — идентификатор обзора;
- ***book_id*** — идентификатор книги;
- ***username*** — имя пользователя, написавшего обзор;
- ***text*** — текст обзора.

### Задача

- Посчитать, сколько книг вышло после 1 января 2000 года;
- Для каждой книги посчитать количество обзоров и среднюю оценку;
- Определить издательство, которое выпустило наибольшее число книг толще 50 страниц — так исключаем из анализа брошюры;
- Определить автора с самой высокой средней оценкой книг — учитывать только книги с 50 и более оценками;
- Посчитайте среднее количество обзоров от пользователей, которые поставили больше 48 оценок.

### Используемые библиотеки

*pandas*  
*sqlalchemy*  
