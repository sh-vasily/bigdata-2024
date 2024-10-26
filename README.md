# bigdata-2024

# Лекция 1.  Что такое "Большие данные". Отличия реляционных от нереляционных баз данных.

- [Материалы](https://disk.yandex.ru/d/wYZ5KCF9_L62Zg)

# Лекция 2. Знакомство с платформой и дистрибутивами Hadoop

- [Материалы](https://disk.yandex.ru/d/YgiWHB6JPOve4Q)

# Лекция 3.  Платформа Apache Hadoop: файловая система HDFS. Форматы хранения данных. Компрессия данных.

- [Материалы](https://disk.yandex.ru/d/G6SE3v_-FtsV9A)

# Лекция 4. Планировщик задач YARN

- [Материалы](https://disk.yandex.ru/d/s43-FX-eOoZqOA)

# Лекция 5. Фреймворк Apache Spark

- [Материалы](https://disk.yandex.ru/d/WTGaC4nEMtcW8g)

- [Исходный код](spark/pyspark.ipynb)

# Лекция 6.

# Лекция 7.

# Лекция 8.

# Задание(реализовать на apache spark в режиме in memory)

Постановка задачи: Выбрать вариант, реалиовать запросы на pyspark/java/scala

Ссылка на датасеты: https://data.who.int/dashboards/covid19/data?n=c

Шаги: 
1. Загрузить csv датасет(согласно варианту) в spark
2. Проверить корректность загруженных данных c помощью spark (количество строк, корректность заполнения всех столбцов).
3. Реализовать запрос согласно варианту.

Решение можно отправить в виде иходного кода или jupyter notebook в телеграм sh_vasily либо на почту basil.scherbakov@ya.ru

Вариант 1:
- Датасет DAILY_CASES (Daily COVID-19 cases and deaths by date reported to WHO)
- запрос 1: вывести top 10 стран с наибольшей смертностью за 2023 год в формате: Country, Deaths
- запрос 2: вывести top 10 стран и месяцев с наибольшей скоростью распространения заболевания за 2023 год в формате: Country, Month, Cases_velocity

Вариант 2: COVID_VAC_META (COVID-19 vaccine introduction data (formerly: "COVID-19 vaccination metadata"))
- запрос 1: вывести страны, в которых доступно наибольшее количество вакцин (ISO3, Number_of_vaccines).
- запрос 2: вывести top 5 вакцин по количеству стран, где они применяются (VACCINE_NAME, Number_of_countries)

Вариант 3:
- Датасеты 
      COVID_VAC_META (COVID-19 vaccine introduction data (formerly: "COVID-19 vaccination metadata")), 
      COVID_VAC (COVID-19 vaccination data)
- запрос: Вывести список вакцин и оценку количества введенных доз (VACCINE_NAME, TOTAL_VACCINATIONS).
Если в стране используется несколько вакцин - можно считать, что они применяются в равных долях.

Вариант 4: 
- Датасеты DAILY_CASES (Daily COVID-19 cases and deaths by date reported to WHO), COUNTRIES (https://en.wikipedia.org/wiki/List_of_countries_and_dependencies_by_population_density)
- запрос: Определить, насколько скорость распространения COVID зависит от плотности населения страны.


Материалы:
- https://mai.moscow/pages/viewpage.action?pageId=14155796
- https://github.com/sh-vasily/bigdata-2023/tree/main/spark
