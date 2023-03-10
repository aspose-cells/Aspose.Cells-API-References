---
title: CellsHelper класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 230
url: /ru/python-net/aspose.cells/cellshelper/
is_root: false
---
##  CellsHelper класс
Предоставляет вспомогательные функции.



Тип CellsHelper предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [significant_digits](/cells/ru/python-net/aspose.cells/cellshelper/significant_digits) | Получает и задает количество значащих цифр.<br/> Значение по умолчанию — 17.|
| [dpi](/cells/ru/python-net/aspose.cells/cellshelper/dpi) | Получает DPI машины.|
| [startup_path](/cells/ru/python-net/aspose.cells/cellshelper/startup_path) |Получает или задает путь запуска, на который ссылаются некоторые внешние ссылки на формулы.|
| [alt_start_path](/cells/ru/python-net/aspose.cells/cellshelper/alt_start_path) | Получает или задает альтернативный путь запуска, на который ссылаются некоторые внешние ссылки на формулы.|
| [library_path](/cells/ru/python-net/aspose.cells/cellshelper/library_path) | Получает или задает путь к библиотеке, на который ссылаются некоторые внешние ссылки на формулы.|
| [custom_implementation_factory](/cells/ru/python-net/aspose.cells/cellshelper/custom_implementation_factory) | Получает или задает фабрику для создания экземпляров со специальной реализацией.|
| [is_cloud_platform](/cells/ru/python-net/aspose.cells/cellshelper/is_cloud_platform) | Установите для этого свойства значение True при работе на облачной платформе, такой как Azure, AWSLambda и т. д.|


###  Методы
| Метод| Описание|
| :- | :- |
| [create_safe_sheet_name(name_proposal)](/cells/ru/python-net/aspose.cells/cellshelper/create_safe_sheet_name/#str) | Проверяет заданное имя листа и при необходимости создает допустимое.<br/>Если данное имя листа соответствует правилам имени листа Excel, верните его.<br/>В противном случае строка будет усечена, если длина превысит лимит<br/> и недопустимые символы будут заменены на ' ', а затем вернут перестроенное строковое значение.|
| [create_safe_sheet_name(name_proposal, replace_char)](/cells/ru/python-net/aspose.cells/cellshelper/create_safe_sheet_name/#str-char) | Проверяет заданное имя листа и при необходимости создает допустимое.<br/>Если данное имя листа соответствует правилам имени листа Excel, верните его.<br/>В противном случае строка будет усечена, если длина превысит лимит<br/> и недопустимые символы будут заменены заданным символом, а затем вернут перестроенное строковое значение.|
| [get_text_width(text, font, scaling)](/cells/ru/python-net/aspose.cells/cellshelper/get_text_width/#str-Font-float) | Получить ширину текста в пунктах.|
| [get_version()](/cells/ru/python-net/aspose.cells/cellshelper/get_version/#) | Получить релизную версию.|
| [cell_name_to_index(cell_name, row, column)](/cells/ru/python-net/aspose.cells/cellshelper/cell_name_to_index/#str-any-any) | Получает индексы строки и столбца ячейки в соответствии с ее именем.|
| [cell_index_to_name(row, column)](/cells/ru/python-net/aspose.cells/cellshelper/cell_index_to_name/#int-int) | Получает имя ячейки в соответствии с ее индексами строки и столбца.|
| [column_index_to_name(column)](/cells/ru/python-net/aspose.cells/cellshelper/column_index_to_name/#int) | Получает имя столбца по индексу столбца.|
| [column_name_to_index(column_name)](/cells/ru/python-net/aspose.cells/cellshelper/column_name_to_index/#str) |Получает индекс столбца в соответствии с именем столбца.|
| [row_index_to_name(row)](/cells/ru/python-net/aspose.cells/cellshelper/row_index_to_name/#int) | Получает имя строки в соответствии с индексом строки.|
| [row_name_to_index(row_name)](/cells/ru/python-net/aspose.cells/cellshelper/row_name_to_index/#str) | Получает индекс строки в соответствии с именем строки.|
| [convert_r1c1_formula_to_a1(r_1c1_formula, row, column)](/cells/ru/python-net/aspose.cells/cellshelper/convert_r1c1_formula_to_a1/#str-int-int) | Преобразует формулу r1c1 ячейки в формулу A1.|
| [convert_a1_formula_to_r1c1(formula, row, column)](/cells/ru/python-net/aspose.cells/cellshelper/convert_a1_formula_to_r1c1/#str-int-int) | Преобразует формулу ячейки A1 в формулу r1c1.|
| [get_date_time_from_double(double_value, date1904)](/cells/ru/python-net/aspose.cells/cellshelper/get_date_time_from_double/#float-bool) | Преобразуйте двойное значение в значение даты и времени.|
| [get_double_from_date_time(date_time, date1904)](/cells/ru/python-net/aspose.cells/cellshelper/get_double_from_date_time/#DateTime-bool) | Преобразуйте дату и время в двойное значение.|
| [get_used_colors(workbook)](/cells/ru/python-net/aspose.cells/cellshelper/get_used_colors/#Workbook) | Получает все используемые цвета в книге.|
| [add_add_in_function(function, min_count_of_parameters, max_count_of_parameters, paramers_type, function_value_type)](/cells/ru/python-net/aspose.cells/cellshelper/add_add_in_function/#str-int-int-list-ParameterType) | Добавить функцию надстройки.|
| [merge_files(files, cached_file, dest_file)](/cells/ru/python-net/aspose.cells/cellshelper/merge_files/#list-str-str) | Объединяет несколько больших файлов xls в файл xls.|
| [init_for_dot_net_core()](/cells/ru/python-net/aspose.cells/cellshelper/init_for_dot_net_core/#) | Выполните инициализацию программы .NetCore.<br/> Мы предлагаем вам сначала вызывать этот метод для всех инициализаций .NetCore.<br/>Например:<br/>CellsHelper.InitForDotNetCore();<br/> Рабочая книга wb = новая рабочая книга();|



###  Смотрите также
* модуль [aspose.cells](..)
