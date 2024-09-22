В данном проекте были решены задачи по исследованию нескольких аспектов мобильного приложения компании, разрабатывающей мобильные игры.

Работа выполнена на Python с использованием Jupyter Notebook.

<p> Задание 1 </p>  
Retention – один из самых важных показателей в компании. Ваша задача – написать функцию, которая будет считать retention игроков (по дням от даты регистрации игрока). Данные лежат в папке shared и имеют следующую структуру:

- shared/problem1-reg_data.csv – данные о времени регистрации

| reg_ts  | Uid |
| ------------- | ------------- |
| 906166566  | 2  |
| 906344325  | 2  |
| 906686169  | 2 |
| 906893386  | 2  |
| 906980227  | 2  |

- shared/problem1-auth_data.csv – данные о времени захода пользователей в игру

| auth_ts  | Uid |
| ------------- | ------------- |
| 906166566  | 2  |
| 924422172  | 3  |
| 937374732  | 4 |
| 947425117  | 5  |
| 955630339  | 6  |

<p> Задание 2 </p>
Имеются результаты A/B теста, в котором двум группам пользователей предлагались различные наборы акционных предложений. Известно, что ARPU в тестовой группе выше на 5%, чем в контрольной. При этом в контрольной группе 1928 игроков из 202103 оказались платящими, а в тестовой – 1805 из 202667.

Какой набор предложений можно считать лучшим? Какие метрики стоит проанализировать для принятия правильного решения и как?
Формат данных:
| user_id  | revenue | testgroup |
| ------------- | ------------- | ------------- |
| 1  | 0  | b |
| 2  | 0  | a |
| 3  | 0 | a |
| 4  | 0  | b |
| 5  | 0  | b |

<p> Задание 3 </p>  
В игре Plants & Gardens каждый месяц проводятся тематические события, ограниченные по времени. В них игроки могут получить уникальные предметы для сада и персонажей, дополнительные монеты или бонусы. Для получения награды требуется пройти ряд уровней за определенное время. С помощью каких метрик можно оценить результаты последнего прошедшего события?

Предположим, в другом событии мы усложнили механику событий так, что при каждой неудачной попытке выполнения уровня игрок будет откатываться на несколько уровней назад. Изменится ли набор метрик оценки результата? Если да, то как?


<p> Реализация проекта: </p>  

- Провел предварительный анализ (EDA) и предобработку данных;
- Написал функцию для расчета Retention игроков;
- Использовал API для загрузки датасетов c яндекс-диска.
- Посчитал и проанализировала продуктовые метрики (Conversion Rate, ARPPU, ARPU).
- Проверил гипотезы, проанализировал результаты А/B-теста с использованием статистических тестов в Python(T-test для ARPU и ARPPU, Хи-квадрат для Conversion Rate).
- Визуализировала результаты в Python с применением seaborn и matplotlib.pyplot.
- Выбрал метрики для оценки результатов последнего прошедшего тематического события игры Plants & Gardens в компании, разрабатывающей мобильные игры и ранжировал их.



