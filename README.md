ДЗ № 2
Домашнее задание к лекции "Введение в типы данных и циклы. Часть 1"
Задание 1
Дана переменная, в которой хранится слово из латинских букв. Напишите код, который выводит на экран:

среднюю букву, если число букв в слове нечетное;
две средних буквы, если число букв четное.
Примеры работы программы:

word = 'test'
Результат:
es

word = 'testing'
Результат:
t

Задание 2
Напишите программу, которая последовательно запрашивает у пользователя числа (по одному за раз) и после первого нуля выводит сумму всех ранее введенных чисел.

Примеры работы программы:
1.

Введите число:  
1

Введите число:  
4

Введите число:  
6

Введите число:  
0
Результат:
11

Введите число:  
0
Результат:
0

Задание 3
Мы делаем MVP dating-сервиса, и у нас есть список парней и девушек.
Выдвигаем гипотезу: лучшие рекомендации мы получим, если просто отсортируем имена по алфавиту и познакомим людей с одинаковыми индексами после сортировки! Но мы не будем никого знакомить, если кто-то может остаться без пары:

Примеры работы программы:
1.

boys = ['Peter', 'Alex', 'John', 'Arthur', 'Richard']
girls = ['Kate', 'Liza', 'Kira', 'Emma', 'Trisha']
Результат:

Идеальные пары:  
Alex и Emma  
Arthur и Kate  
John и Kira  
Peter и Liza  
Richard и Trisha 
boys = ['Peter', 'Alex', 'John', 'Arthur', 'Richard', 'Michael']
girls = ['Kate', 'Liza', 'Kira', 'Emma', 'Trisha']
Результат:
Внимание, кто-то может остаться без пары!

Задание 4
У нас есть список, содержащий информацию о среднедневной температуре в Фаренгейтах за произвольный период по странам (структура данных в примере). Необходимо написать код, который рассчитает среднюю температуру за период в Цельсиях(!) для каждой страны.

Пример работы программы:

countries_temperature = [
    ['Таиланд', [75.2, 77, 78.8, 73.4, 68, 75.2, 77]],
    ['Германия', [57.2, 55.4, 59, 59, 53.6]],
    ['Россия', [35.6, 37.4, 39.2, 41, 42.8, 39.2, 35.6]],
    ['Польша', [50, 50, 53.6, 57.2, 55.4, 55.4]]
]
Результат:

Средняя температура в странах:
Таиланд  -  23.9 С
Германия  -  13.8 С
Россия  -  3.7 С
Польша  -  12.0 С
Задание 5 (необязательное)
Имеется список с транспортными номерами. Необходимо написать код, который проверит каждый номер на валидность (1 буква, 3 цифры, 2 буквы, 2-3 цифры). Обратите внимание, что не все буквы кириллического алфавита используются в транспортных номерах.

Если номер валиден, то вывести его в нужном формавте (пример ниже), а если не валиден — вывести текст. При решении помогут регулярные выражения, с которыми будет знакомство на практике.

Примеры работы программы:

car_ids = ['А222ВС96', 'АБ22ВВ193']

Результат:

Номер А222ВС валиден. Регион: 96
Номер АБ22ВВ193 не валиден
Задание 6 (необязательное)
Дан поток логов по количеству просмотренных страниц для каждого пользователя (пользователь,дата;просмотры). Вам необходимо написать алгоритм, который считает среднее значение просмотров на пользователя. Т. е. надо посчитать отношение суммы всех просмотров к количеству уникальных пользователей. И тут регулярные выражения облегчат немного реализацию.

Примеры работы программы:
1.

stream = [
    'user4,2021-01-01;3',
    'user3,2022-01-07;4',
    'user2,2022-03-29;1',
    'user1,2020-04-04;13',
    'user2,2022-01-05;7',
    'user1,2021-06-14;4',
    'user3,2022-07-02;10',
    'user4,2021-03-21;19',
    'user4,2022-03-22;4',
    'user4,2022-04-22;8',
    'user4,2021-05-03;9',
    'user4,2022-05-11;11'
]
Результат:
Среднее количество просмотров на уникального пользователя: 23.25

stream = [
    'user100,2022-01-01;150',
    'user99,2022-01-07;205',
    'user1001,2022-03-29;81'
]
Результат:
Среднее количество просмотров на уникального пользователя: 145.33

ПРИМЕЧАНИЕ
Домашнее задание сдается ссылкой Google Colab. Не сможем проверить или помочь, если вы пришлете:

файлы;
архивы;
скриншоты кода.
Все обсуждения и консультации по выполнению домашнего задания ведутся только на соответствующем канале в Discord.

Как правильно задавать вопросы аспирантам, преподавателям и коллегам
Прежде чем задать вопрос, попробуйте найти ответ в интернете. Навык самостоятельного поиска информации — один из важнейших. Каждый практикующий специалист любого уровня делает это ежедневно.

Сформулируйте вопрос по алгоритму:

Что я делаю?
Какого результата я ожидаю?
Как фактический результат отличается от ожидаемого?
Что я уже попробовал сделать, чтобы исправить проблему?
По возможности прикрепите к вопросу скриншоты либо ссылки на код. Не выкладывайте все решение, оставляйте только проблемный и воспроизводимый участок кода.



ДЗ №1
Домашнее задание к лекции "Основы Python"
Задание 1
Даны 2 переменных, в которых хранятся строки произвольной длины: phrase_1 и phrase_2.
Напишите код, который проверяет какая из этих строк длиннее.

Примеры работы программы:
1.

phrase_1 = 'Насколько проще было бы писать программы, если бы не заказчики'
phrase_2 = '640Кб должно хватить для любых задач. Билл Гейтс (по легенде)'

Результат:
Фраза 1 длиннее фразы 2 2.

phrase_1 = '640Кб должно хватить для любых задач. Билл Гейтс (по легенде)'
phrase_2 = 'Насколько проще было бы писать программы, если бы не заказчики'
Результат:
Фраза 2 длиннее фразы 1 3.

phrase_1 = 'Насколько проще было бы писать программы, если бы не заказчики'
phrase_2 = 'Насколько проще было бы писать программы, если бы не заказчики'
Результат:
Фразы равной длины

Задание 2
Дана переменная, в которой хранится число (год). Необходимо написать программу, которая выведет, является ли данный год високосным или обычным.

Пример работы программы: 1.

year = 2020
Результат:
Високосный год

year = 2019
Результат:
Обычный год

Задание 3
Необходимо написать программу, которая будет запрашивать у пользователя месяц и дату рождения и выводить соответствующий знак зодиака.

Пример работы программы:
1.

Введите день:
30

Введите месяц:
Август
Результат:
Ваш знак зодиака: Дева

Введите день:
29

Введите месяц:
Октябрь
Результат:
Ваш знак зодиака: Скорпион

Задание 4
Вам нужно написать программу для подбора упаковок по размерам товара. Размеры (ширина, длина, высота) хранятся в переменных (в сантиметрах):

Используйте следующие правила:

если каждое из трех измерений менее или равно 15 сантиметрам, то выведите на экран "Коробка №1";
если хотя бы одно из измерений больше 2 метров, то выводите "Упаковка для лыж";
если хотя бы одно из измерений больше 15 сантиметров, но менее 50 сантиметров, то выводите "Коробка №2";
во всех остальных случаях выводите "Коробка №3".
Пример работы программы:
1.

width = 15
length = 55
height = 15
Результат:
Коробка №3

width = 45
length = 205
height = 45
Результат:
Упаковка для лыж

Задание 5 (необязательное)
Дана переменная, в которой хранится шестизначное число (номер проездного билета). Напишите программу, которая будет определять, является ли данный билет "счастливым". Билет считается счастливым, если сумма первых трех цифр совпадает с суммой последних трех цифр номера.

Примеры работы программы:

number = 123456
Результат:
Несчастливый билет

number = 123321
Результат:
Счастливый билет

Задание 6 (необязательное)
Напишите программу, которая сможет вычислять площади трех фигур (круг, треугольник и прямоугольник). Тип фигуры запрашиваем через пользовательский ввод, после чего делаем запрос характеристик фигуры:

если пользователь выбрал круг, запрашиваем его радиус,
если треугольник – длины трех его сторон;
если прямоугольник – длины двух его сторон.
Пример работы программы:
1.

Введите тип фигуры:
Круг

Введите радиус круга:
10
Результат:
Площадь круга: 314.16

Введите тип фигуры:
Треугольник

Введите длину стороны A:
2

Введите длину стороны B:
2

Введите длину стороны C:
3
Результат:
Площадь треугольника: 1.98

ПРИМЕЧАНИЕ
Домашнее задание сдается ссылкой Google Colab. Не сможем проверить или помочь, если вы пришлете:

файлы;
архивы;
скриншоты кода.
Все обсуждения и консультации по выполнению домашнего задания ведутся только на соответствующем канале в Discord.

Как правильно задавать вопросы аспирантам, преподавателям и коллегам
Прежде чем задать вопрос, попробуйте найти ответ в интернете. Навык самостоятельного поиска информации — один из важнейших. Каждый практикующий специалист любого уровня делает это ежедневно.

Сформулируйте вопрос по алгоритму:

Что я делаю?
Какого результата я ожидаю?
Как фактический результат отличается от ожидаемого?
Что я уже попробовал сделать, чтобы исправить проблему?
По возможности прикрепите к вопросу скриншоты либо ссылки на код. Не выкладывайте все решение, оставляйте только проблемный и воспроизводимый участок кода.
