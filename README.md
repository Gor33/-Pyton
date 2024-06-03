ДЗ № 7 к Лекции "Понятие класс"
Домашнее задание

Задание 1
Напишите функцию, которая возвращает название валюты (поле ‘Name’) с максимальным значением курса с помощью сервиса www.cbr-xml-daily.ru...ly_json.js

Задание 2
Добавьте в класс Rate параметр diff (со значениями True или False), который в случае значения True в методах курсов валют (eur, usd итд) будет возвращать не курс валюты, а изменение по сравнению в прошлым значением. Считайте, self.diff будет принимать значение True только при возврате значения курса. При отображении всей информации о валюте он не используется.

Задание 3
Напишите класс Designer, который учитывает количество международных премий. Подсказки в коде занятия (“Ноутбук к лекциям «Понятие класса» + презентация”, zip-файл “Используемый ноутбук к лекциям «Понятие класса»).

Комментарий по классу Designer такой:
Напишите класс Designer, который учитывает количество международных премий для дизайнеров (из презентации: “Повышение на 1 грейд за каждые 7 баллов. Получение международной премии – это +2 балла”). Считайте, что при выходе на работу сотрудник уже имеет две премии и их количество не меняется со стажем (конечно если хотите это можно вручную менять).

Класс Designer пишется по аналогии с классом Developer из материалов занятия.

ДЗ № 6 к лекции «Исключения и обработка ошибок»
Задание
Вопросы по заданию
Преподаватель: Константин Башевой
Задание 1
Печатные газеты использовали свой формат дат для каждого выпуска. Для каждой газеты из списка напишите формат указанной даты для перевода в объект datetime:
The Moscow Times — Wednesday, October 2, 2002
The Guardian — Friday, 11.10.13
Daily News — Thursday, 18 August 1977

Задание 2
Дан поток дат в формате YYYY-MM-DD, в которых встречаются некорректные значения:
stream = [‘2018-04-02’, ‘2018-02-29’, ‘2018-19-02’]

Напишите функцию, которая проверяет эти даты на корректность. То есть для каждой даты возвращает True — дата корректна или False — некорректная.

Задание 3
Напишите функцию date_range, которая возвращает список дат за период от start_date до end_date. Даты должны вводиться в формате YYYY-MM-DD. В случае неверного формата или при start_date > end_date должен возвращаться пустой список.

Задание 4 (необязательное)
Ваш коллега прислал код функции:

DEFAULT_USER_COUNT = 3

def delete_and_return_last_user(region, default_list=[‘A100’, ‘A101’, ‘A102’]):
""“
Удаляет из списка default_list последнего пользователя
и возвращает ID нового последнего пользователя.
”""
element_to_delete = default_list[-1]
default_list.remove(element_to_delete)

1
return default_list[DEFAULT_USER_COUNT-2]
При однократном вызове этой функции всё работает корректно:
delete_and_return_last_user(1)
‘A101’

Однако при повторном вызове получается ошибка IndexError: list index out of range.

Задание:

Что значит ошибка list index out of range?
Почему при первом запуске функция работает корректно, а при втором — нет?
Важно: замечание к заданию

**** Для зачёта достаточно сделать три задания, четвёртое необязательное.****

При копировании с сайта Нетологии Jupyter ноутбук изменяет кавычки ’ на `. Прошу учесть это и обращать внимание.
Достаточно просто заменить кавычки.

Примечание
Домашнее задание сдаётся ссылкой Google Colab или на репозиторий GitHub, но только если вы знакомы с Git и устанавливали ПО.
Мы не сможем его проверить или помочь, если вы пришлёте:

файлы,
архивы,
скриншоты кода.
Все обсуждения и консультации по выполнению домашнего задания ведутся только на соответствующем канале в Discord.

Как правильно задавать вопросы аспирантам, преподавателям и коллегам
Прежде чем задать вопрос, необходимо попробовать найти ответ самому в интернете. Навык самостоятельного поиска информации — один из важнейших, и каждый практикующий специалист любого уровня делает это каждый день.

Любой вопрос должен быть сформулирован по алгоритму:

Что я делаю?
Какого результата я ожидаю?
Как фактический результат отличается от ожидаемого?
Что я уже попробовал сделать, чтобы исправить проблему?
По возможности прикрепляйте к вопросу скриншоты либо ссылки на код. Оставляйте только проблемный и воспроизводимый участок кода, всё решение выкладывать не допускается.


ДЗ № 5
Домашнее задание
1.	Переведите содержимое файла purchase_log.txt* в словарь purchases вида:
{‘1840e0b9d4’: ‘Продукты’, …}

2.	Для каждого user_id в файле visit_log.csv определите третий столбец с категорией покупки, если покупка была, сам файл visit_log.csv* изменять не надо. Запишите в файл funnel.csv визиты из файла visit_log.csv*, в которых были покупки с указанием категории.

Учтите условия на данные:
содержимое purchase_log.txt* помещается в оперативную память компьютера;
содержимое visit_log.csv* — нет; используйте только построчную обработку этого файла.

*Все файлы, необходимые для выполнения домашнего задания, находятся в разделе “Дополнительные материалы к домашнему заданию” (нужно скачать архив).

Примечание
Домашнее задание сдаётся ссылкой Google Colab или на репозиторий GitHub, но только если вы знакомы с Git и устанавливали ПО.
Мы не сможем его проверить или помочь, если вы пришлёте:
файлы,
архивы,
скриншоты кода.
Все обсуждения и консультации по выполнению домашнего задания ведутся только на соответствующем канале в Discord.

Как правильно задавать вопросы аспирантам, преподавателям и коллегам
Прежде чем задать вопрос, необходимо попробовать найти ответ самому в интернете. Навык самостоятельного поиска информации — один из важнейших, и каждый практикующий специалист любого уровня делает это каждый день.

Любой вопрос должен быть сформулирован по алгоритму:

Что я делаю?
Какого результата я ожидаю?
Как фактический результат отличается от ожидаемого?
Что я уже попробовал сделать, чтобы исправить проблему?


ДЗ № 4
Домашнее задание к лекции «Функции»

Содержание ДЗ можно изучить здесь.

Вам нужно помочь секретарю автоматизировать работу. Для этого нужно написать программу, которая будет на основе хранимых данных исполнять пользовательские команды.

Исходные данные имеют следующую структуру:

Перечень всех документов.
documents = [
{‘type’: ‘passport’, ‘number’: ‘2207 876234’, ‘name’: ‘Василий Гупкин’},
{‘type’: ‘invoice’, ‘number’: ‘11-2’, ‘name’: ‘Геннадий Покемонов’},
{‘type’: ‘insurance’, ‘number’: ‘10006’, ‘name’: ‘Аристарх Павлов’}
]
Перечень полок, на которых хранятся документы. Если документ есть в documents, то он обязательно должен быть и в directories.
directories = {
‘1’: [‘2207 876234’, ‘11-2’],
‘2’: [‘10006’],
‘3’: []
}
Общие требования к программе:
код должен быть грамотно декомпозирован: каждая функция отвечает за свою конкретную задачу, дублирующийся функционал переиспользуется, а его код не повторяется;
в коде отсутствуют глобальные переменные, за исключением documents и directories;
пользовательский ввод обрабатывается в цикле while до тех пор, пока пользователь явно не завершит программу вводом команды «q».
**Задание 1
Пункт 1. Пользователь по команде «p» может узнать владельца документа по его номеру.
Примеры работы:

Введите команду:
p

Введите номер документа:
10006
Результат:
Владелец документа: Аристарх Павлов

Введите команду:
p

Введите номер документа:
12345
Результат:
Документ не найден в базе

Пункт 2. Пользователь по команде «s» может по номеру документа узнать, на какой полке он хранится.
Примеры работы:

Введите команду:
s

Введите номер документа:
10006
Результат:
Документ хранится на полке: 2

Введите команду:
s

Введите номер документа:
12345
Результат:
Документ не найден в базе

Пункт 3. Пользователь по команде «l» может увидеть полную информацию по всем документам.
Пример работы:

Введите команду:
l
Результат:

№: 2207 876234, тип: passport, владелец: Василий Гупкин, полка хранения: 1
№: 11-2, тип: invoice, владелец: Геннадий Покемонов, полка хранения: 1
№: 10006, тип: insurance, владелец: Аристарх Павлов, полка хранения: 2

Пункт 4. Пользователь по команде «ads» может добавить новую полку.
Примеры работы:

Введите команду:
ads

Введите номер полки:
10
Результат:
Полка добавлена. Текущий перечень полок: 1, 2, 3, 10.

Введите команду:
ads

Введите номер полки:
1
Результат:
Такая полка уже существует. Текущий перечень полок: 1, 2, 3.

Пункт 5. Пользователь по команде «ds» может удалить существующую полку из данных, только если она пустая.
Примеры работы:

Введите команду:
ds

Введите номер полки:
3
Результат:
Полка удалена. Текущий перечень полок: 1, 2.

Введите команду:
ds

Введите номер полки:
1
Результат:
На полке есть документы, удалите их перед удалением полки. Текущий перечень полок: 1, 2, 3.

Введите команду:
ds

Введите номер полки:
4
Результат:
Такой полки не существует. Текущий перечень полок: 1, 2, 3.

Задание 2 (необязательное)
Вам необходимо дополнить программу из задания 1 более продвинутыми командами.

Пункт 1. Пользователь по команде «ad» может добавить новый документ в данные.
Примеры работы:

Введите команду:
ad

Введите номер документа:
42
Введите тип документа:
multipassport
Введите владельца документа:
R2D2
Введите полку для хранения:
3
Результат:

Документ добавлен. Текущий список документов:
№: 2207 876234, тип: passport, владелец: Василий Гупкин, полка хранения: 1
№: 11-2, тип: invoice, владелец: Геннадий Покемонов, полка хранения: 1
№: 10006, тип: insurance, владелец: Аристарх Павлов, полка хранения: 2
№: 42, тип: multipassport, владелец: R2D2, полка хранения: 3
2.

Введите команду:
ad

Введите номер документа:
42
Введите тип документа:
multipassport
Введите владельца документа:
R2D2
Введите полку для хранения:
4
Результат:

Такой полки не существует. Добавьте полку командой as.
Текущий список документов:
№: 2207 876234, тип: passport, владелец: Василий Гупкин, полка хранения: 1
№: 11-2, тип: invoice, владелец: Геннадий Покемонов, полка хранения: 1
№: 10006, тип: insurance, владелец: Аристарх Павлов, полка хранения: 2

Пункт 2. Пользователь по команде «d» может удалить документ из данных.
Примеры работы:

Введите команду:
d

Введите номер документа:
10006
Результат:

Документ удалён.
Текущий список документов:
№: 2207 876234, тип: passport, владелец: Василий Гупкин, полка хранения: 1
№: 11-2, тип: invoice, владелец: Геннадий Покемонов, полка хранения: 1
2.

Введите команду:
d

Введите номер документа:
123456
Результат:

Документ не найден в базе.
Текущий список документов:
№: 2207 876234, тип: passport, владелец: Василий Гупкин, полка хранения: 1
№: 11-2, тип: invoice, владелец: Геннадий Покемонов, полка хранения: 1
№: 10006, тип: insurance, владелец: Аристарх Павлов, полка хранения: 2

Пункт 3. Пользователь по команде «m» может переместить документ с полки на полку.
Примеры работы:

Введите команду:
m

Введите номер документа:
11-2
Введите номер полки:
3
Результат:

Документ перемещён.
Текущий список документов:
№: 2207 876234, тип: passport, владелец: Василий Гупкин, полка хранения: 1
№: 11-2, тип: invoice, владелец: Геннадий Покемонов, полка хранения: 3
№: 10006, тип: insurance, владелец: Аристарх Павлов, полка хранения: 2
2.

Введите команду:
m

Введите номер документа:
11-2
Введите номер полки:
10
Результат:
Такой полки не существует. Текущий перечень полок: 1, 2, 3.

Введите команду:
m

Введите номер документа:
42
Введите номер полки:
2
Результат:

Документ не найден в базе.
Текущий список документов:
№: 2207 876234, тип: passport, владелец: Василий Гупкин, полка хранения: 1
№: 11-2, тип: invoice, владелец: Геннадий Покемонов, полка хранения: 1
№: 10006, тип: insurance, владелец: Аристарх Павлов, полка хранения: 2

Примечание
Домашнее задание сдаётся ссылкой Google Colab или на репозиторий GitHub, но только если вы знакомы с Git и устанавливали ПО.
Мы не сможем его проверить или помочь, если вы пришлёте:

файлы,
архивы,
скриншоты кода.
Все обсуждения и консультации по выполнению домашнего задания ведутся только на соответствующем канале в Discord.

Как правильно задавать вопросы аспирантам, преподавателям и коллегам
Прежде чем задать вопрос, необходимо попробовать найти ответ самому в интернете. Навык самостоятельного поиска информации — один из важнейших, и каждый практикующий специалист любого уровня делает это каждый день.

Любой вопрос должен быть сформулирован по алгоритму:

Что я делаю?
Какого результата я ожидаю?
Как фактический результат отличается от ожидаемого?
Что я уже попробовал сделать, чтобы исправить проблему?
По возможности прикрепляйте к вопросу скриншоты либо ссылки на код. Оставляйте только проблемный и воспроизводимый участок кода, всё решение выкладывать не допускается.
ДЗ № 3
Домашнее задание к лекции "Введение в типы данных и циклы. Часть 2"
Задание 1
Дана переменная, в которой хранится словарь, содержащий гео-метки для каждого пользователя (пример структуры данных приведен ниже). Вам необходимо написать программу, которая выведет на экран множество уникальных гео-меток всех пользователей.

Пример работы программы:

ids = {'user1': [213, 213, 213, 15, 213], 
       'user2': [54, 54, 119, 119, 119], 
       'user3': [213, 98, 98, 35]}
Результат: {98, 35, 15, 213, 54, 119}

Задание 2
Дана переменная, в которой хранится список поисковых запросов пользователя (пример структуры данных приведен ниже, но запросы потенциально могут быть любые). Вам необходимо написать программу, которая выведет на экран распределение количества слов в запросах в требуемом виде.

Пример работы программы:

queries = [
    'смотреть сериалы онлайн',
    'новости спорта',
    'афиша кино',
    'курс доллара',
    'сериалы этим летом',
    'курс по питону',
    'сериалы про спорт',
]
Результат:

Поисковых запросов, содержащих 2 слов(а): 42.86%
Поисковых запросов, содержащих 3 слов(а): 57.14%
Задание 3
Дана переменная, в которой хранится информация о затратах и доходе рекламных кампаний по различным источникам. Необходимо дополнить исходную структуру показателем ROI, который рассчитаем по формуле: ((revenue / cost) - 1) * 100

Пример работы программы:

results = {
    'vk': {'revenue': 103, 'cost': 98},
    'yandex': {'revenue': 179, 'cost': 153},
    'facebook': {'revenue': 103, 'cost': 110},
    'adwords': {'revenue': 35, 'cost': 34},
    'twitter': {'revenue': 11, 'cost': 24},
}
Результат:

{'adwords': {'revenue': 35, 'cost': 34, 'ROI': 2.94},
 'facebook': {'revenue': 103, 'cost': 110, 'ROI': -6.36},
 'twitter': {'revenue': 11, 'cost': 24, 'ROI': -54.17},
 'vk': {'revenue': 103, 'cost': 98, 'ROI': 5.1},
 'yandex': {'revenue': 179, 'cost': 153, 'ROI': 16.99}}
Задание 4
Дана переменная, в которой хранится статистика рекламных каналов по объемам продаж (пример структуры данных приведен ниже). Напишите программу, которая возвращает название канала с максимальным объемом продаж.

Пример работы программы:

stats = {'facebook': 55, 'yandex': 115, 'vk': 120, 'google': 99, 'email': 42, 'ok': 98}

Результат: Максимальный объем продаж на рекламном канале: vk

Задание 5 (необязательно)
Дан список произвольной длины. Необходимо написать код, который на основе исходного списка составит словарь такого уровня вложенности, какова длина исхондого списка.

Примеры работы программы:

my_list = ['2018-01-01', 'yandex', 'cpc', 100]
Результат: {'2018-01-01': {'yandex': {'cpc': 100}}}

my_list = ['a', 'b', 'c', 'd', 'e', 'f']
Результат: {'a': {'b': {'c': {'d': {'e': 'f'}}}}}

Задание 6 (необязательно)
Дана книга рецептов с информацией о том, сколько ингредиентов нужно для приготовления блюда в расчете на одну порцию (пример данных представлен ниже).
Напишите программу, которая будет запрашивать у пользователя количество порций для приготовления этих блюд и отображать информацию о суммарном количестве требуемых ингредиентов в указанном виде.
Внимание! Одинаковые ингредиенты с разными размерностями нужно считать раздельно!
Пример работы программы:

cook_book = {
  'салат': [
     {'ingridient_name': 'сыр', 'quantity': 50, 'measure': 'гр'},
     {'ingridient_name': 'томаты', 'quantity': 2, 'measure': 'шт'},
     {'ingridient_name': 'огурцы', 'quantity': 20, 'measure': 'гр'},
     {'ingridient_name': 'маслины', 'quantity': 10, 'measure': 'гр'},
     {'ingridient_name': 'оливковое масло', 'quantity': 20, 'measure': 'мл'},
     {'ingridient_name': 'салат', 'quantity': 10, 'measure': 'гр'},
     {'ingridient_name': 'перец', 'quantity': 20, 'measure': 'гр'}
    ],
  'пицца': [
     {'ingridient_name': 'сыр', 'quantity': 20, 'measure': 'гр'},
     {'ingridient_name': 'колбаса', 'quantity': 30, 'measure': 'гр'},
     {'ingridient_name': 'бекон', 'quantity': 30, 'measure': 'гр'},
     {'ingridient_name': 'оливки', 'quantity': 10, 'measure': 'гр'},
     {'ingridient_name': 'томаты', 'quantity': 20, 'measure': 'гр'},
     {'ingridient_name': 'тесто', 'quantity': 100, 'measure': 'гр'},   
    ],
  'лимонад': [
     {'ingridient_name': 'лимон', 'quantity': 1, 'measure': 'шт'},
     {'ingridient_name': 'вода', 'quantity': 200, 'measure': 'мл'},
     {'ingridient_name': 'сахар', 'quantity': 10, 'measure': 'гр'},
     {'ingridient_name': 'лайм', 'quantity': 20, 'measure': 'гр'},    
    ]
}

Введите количество порций:  
3
Результат:

Сыр: 210 гр  
Томаты: 6 шт  
Огурцы: 60 гр  
Маслины: 30 гр  
Оливковое масло: 60 мл  
Салат: 30 гр  
Перец: 60 гр  
Колбаса: 90 гр  
Бекон: 90 гр  
Оливки: 30 гр  
Томаты: 60 гр  
Тесто: 300 гр  
Лимон: 3 шт  
Вода: 600 мл  
Сахар: 30 гр  
Лайм: 60 гр  

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
