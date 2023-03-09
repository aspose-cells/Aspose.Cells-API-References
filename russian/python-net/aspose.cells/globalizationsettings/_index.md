---
title: GlobalizationSettings класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 730
url: /ru/python-net/aspose.cells/globalizationsettings/
is_root: false
---
##  GlobalizationSettings класс
Представляет параметры глобализации.



Тип GlobalizationSettings предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [GlobalizationSettings()](/cells/ru/python-net/aspose.cells/globalizationsettings/__init__/#) | Создает новый экземпляр GlobalizationSettings|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [chart_settings](/cells/ru/python-net/aspose.cells/globalizationsettings/chart_settings) | Получает или задает параметры глобализации для Chart.|
| [pivot_settings](/cells/ru/python-net/aspose.cells/globalizationsettings/pivot_settings) | Получает или задает параметры глобализации для сводной таблицы.|
| [list_separator](/cells/ru/python-net/aspose.cells/globalizationsettings/list_separator) | Получает разделитель для списка, параметры функции и т.д.|
| [row_separator_of_formula_array](/cells/ru/python-net/aspose.cells/globalizationsettings/row_separator_of_formula_array) |Получает разделитель для строк в массиве данных в формуле.|
| [column_separator_of_formula_array](/cells/ru/python-net/aspose.cells/globalizationsettings/column_separator_of_formula_array) | Получает разделитель для элементов в данных строки массива в формуле.|


###  Методы
| Метод| Описание|
| :- | :- |
| [get_pivot_total_name()](/cells/ru/python-net/aspose.cells/globalizationsettings/get_pivot_total_name/#) | Получает имя метки «Итого» в сводной таблице.<br/> Вам необходимо переопределить этот метод, если сводная таблица содержит два или более сводных полей в области данных.|
| [get_pivot_grand_total_name()](/cells/ru/python-net/aspose.cells/globalizationsettings/get_pivot_grand_total_name/#) | Получает имя метки «Общий итог» в сводной таблице.|
| [get_multiple_items_name()](/cells/ru/python-net/aspose.cells/globalizationsettings/get_multiple_items_name/#) | Получает имя метки «(Несколько элементов)» в сводной таблице.|
| [get_all_name()](/cells/ru/python-net/aspose.cells/globalizationsettings/get_all_name/#) | Получает имя метки "(Все)" в сводной таблице.|
| [get_protection_name_of_pivot_table()](/cells/ru/python-net/aspose.cells/globalizationsettings/get_protection_name_of_pivot_table/#) | Получает имя защиты в сводной таблице.|
| [get_column_labels_of_pivot_table()](/cells/ru/python-net/aspose.cells/globalizationsettings/get_column_labels_of_pivot_table/#) | Получает имя метки «Метки столбцов» в сводной таблице.|
| [get_row_labels_name_of_pivot_table()](/cells/ru/python-net/aspose.cells/globalizationsettings/get_row_labels_name_of_pivot_table/#) | Получает имя метки «Метки строк» в сводной таблице.|
| [get_empty_data_name()](/cells/ru/python-net/aspose.cells/globalizationsettings/get_empty_data_name/#) | Получает имя метки "(пусто)" в сводной таблице.|
| [get_data_field_header_name_of_pivot_table()](/cells/ru/python-net/aspose.cells/globalizationsettings/get_data_field_header_name_of_pivot_table/#) | Получает имя заголовка поля области значений в сводной таблице.|
| [get_sub_total_name(sub_total_type)](/cells/ru/python-net/aspose.cells/globalizationsettings/get_sub_total_name/#aspose.cells.pivot.PivotFieldSubtotalType) | Получает имя типа [PivotFieldSubtotalType](/cells/ru/python-net/aspose.cells.pivot/pivotfieldsubtotaltype) в сводной таблице.|
| [get_total_name(function_type)](/cells/ru/python-net/aspose.cells/globalizationsettings/get_total_name/#ConsolidationFunction) | Получает полное имя функции.|
| [get_grand_total_name(function_type)](/cells/ru/python-net/aspose.cells/globalizationsettings/get_grand_total_name/#ConsolidationFunction) | Получает общее имя функции.|
| [get_table_row_type_of_headers()](/cells/ru/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_headers/#) | Получает имя типа строк таблицы, состоящее из заголовка таблицы.<br/>По умолчанию используется «Заголовки», поэтому в формуле «#Заголовки» представляет собой заголовок таблицы.|
| [get_table_row_type_of_data()](/cells/ru/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_data/#) | Получает имя типа строк таблицы, состоящей из области данных ссылочной таблицы.<br/> По умолчанию используется «Данные», поэтому в формуле «#Данные» представляет область данных таблицы.|
| [get_table_row_type_of_all()](/cells/ru/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_all/#) | Получает имя типа строк таблицы, состоящее из всех строк в таблице, на которую ссылаются.<br/> По умолчанию используется значение «Все», поэтому в формуле «#Все» представляют все строки в ссылочной таблице.|
| [get_table_row_type_of_totals()](/cells/ru/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_totals/#) | Получает имя типа строк таблицы, состоящее из общей строки таблицы, на которую ссылаются.<br/> По умолчанию используется значение «Итоги», поэтому в формуле «#Итоги» представляет итоговую строку ссылочной таблицы.|
| [get_table_row_type_of_current()](/cells/ru/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_current/#) | Получает имя типа строк таблицы, состоящих из текущей строки в таблице, на которую ссылаются.<br/> По умолчанию используется «Эта строка», поэтому в формуле «# Эта строка» представляет текущую строку в ссылочной таблице.|
| [get_error_value_string(err)](/cells/ru/python-net/aspose.cells/globalizationsettings/get_error_value_string/#str) | Получает отображаемое строковое значение для значения ошибки ячейки|
| [get_boolean_value_string(bv)](/cells/ru/python-net/aspose.cells/globalizationsettings/get_boolean_value_string/#bool) | Получает отображаемое строковое значение для логического значения ячейки|
| [get_local_function_name(standard_name)](/cells/ru/python-net/aspose.cells/globalizationsettings/get_local_function_name/#str) | Получает зависящее от языкового стандарта имя функции в соответствии с заданным стандартным именем функции.|
| [get_standard_function_name(local_name)](/cells/ru/python-net/aspose.cells/globalizationsettings/get_standard_function_name/#str) | Получает стандартное имя функции в соответствии с заданным именем функции, зависящим от локали.|
| [get_local_built_in_name(standard_name)](/cells/ru/python-net/aspose.cells/globalizationsettings/get_local_built_in_name/#str) | Получает зависящий от локали текст для встроенного имени в соответствии с заданным стандартным текстом.|
| [get_standard_built_in_name(local_name)](/cells/ru/python-net/aspose.cells/globalizationsettings/get_standard_built_in_name/#str) | Получает стандартный текст встроенного имени в соответствии с заданным текстом, зависящим от локали.|
| [get_standard_header_footer_font_style_name(localfont_style_name)](/cells/ru/python-net/aspose.cells/globalizationsettings/get_standard_header_footer_font_style_name/#str) | Получает имя стиля стандартного английского шрифта (обычный, полужирный, курсив) для верхнего/нижнего колонтитула в соответствии с заданным именем стиля шрифта локали.|
| [get_comment_title_name(type)](/cells/ru/python-net/aspose.cells/globalizationsettings/get_comment_title_name/#aspose.cells.rendering.CommentTitleType) |Получает зависящее от локали название заголовка комментария в соответствии с типом заголовка комментария.|
| [compare(v1, v2, ignore_case)](/cells/ru/python-net/aspose.cells/globalizationsettings/compare/#str-str-bool) | Сравнивает два строковых значения в соответствии с определенными правилами сортировки.|



###  Смотрите также
* модуль [aspose.cells](..)
* класс [PivotFieldSubtotalType](/cells/ru/python-net/aspose.cells.pivot/pivotfieldsubtotaltype)
