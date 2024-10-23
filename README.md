# bigdata-2024

Задание(реализовать на apache spark в режиме in memory)

Шаги:
1. Проверить корректность загруженных данных через SQL-запрос (количество строк, корректность заполнения всех столбцов).
2. Реализовать SQL запросы согласно варианту.


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
