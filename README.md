# Проект по прогнозированию цен на золото

Warning: на момент промежуточного чекпоинта из загруженных файлов не доделан файл с визуализацией, и частично недоделан файл с EDA (будут заполнены столбцы Key_rate и Inflation)

## Описание проекта

В данном проекте я анализирую цены на золото с 01.09.2013 по 01.01.2025 с целью их дальнейшего прогнозирования на основе модели линейной регрессии. В качестве анализируемых параметров модели я взяла:
* индекс IMOEX - индикатор состояния экономики в целом
* индекс MOEXMM - индикатор объемов добычи металлов
* Данные по инфляции - золото является хэджирующим активом против инфляции, поэтому ожидается высокая корреляция между показателями
* Курс USD_RUB - индикатор разницы между ценами на золото в валюте

Зависимой переменной являются цены на золото.

## Структура проекта

1) Выбор темы
2) Сбор (парсинг данных)
3) Предобработка данных
4) Визуализация и создание новых признаков
5) Тестирование гипотез
6) Машинное обучение
7) Выводы
   
## Навигация по файлам:

1) DA_parsing - файл с парсингом.
В рамках парсинга использовались:
* MOEX API (https://iss.moex.com/iss/reference/). С сайта Московской биржи были спарсены данные IMOEX, MOEXMM;
* XML ЦБ (https://cbr.ru/development/SXML/). С сайта ЦБ были спарсены данные инфляции, валютных пар USDRUB, цен на золото.

2) DA_EDA - файл с предобработкой данных. В рамках неё был совмещены отдельные дата фреймы в единый result_df, заполнены пропуски.

3) DA_Visualization - файл с визуализацией данных и созданием новых параметров для анализа.

   to be continued...
  



