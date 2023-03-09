---
title: ExportTableOptions класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 550
url: /ru/python-net/aspose.cells/exporttableoptions/
is_root: false
---
##  ExportTableOptions класс
Представляет все параметры таблицы экспорта.



Тип ExportTableOptions предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [ExportTableOptions()](/cells/ru/python-net/aspose.cells/exporttableoptions/__init__/#) | Создает новый экземпляр ExportTableOptions|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [export_column_name](/cells/ru/python-net/aspose.cells/exporttableoptions/export_column_name) | Указывает, экспортируются ли данные в первой строке в имя столбца DataTable.<br/> Значение по умолчанию неверно.|
| [skip_error_value](/cells/ru/python-net/aspose.cells/exporttableoptions/skip_error_value) | Указывает, следует ли пропускать недопустимое значение для столбца.<br/> Например, если тип столбца десятичный, значение больше, чем decimal.MaxValue.<br/>и это свойство истинно, мы больше не будем выбрасывать исключение.<br/> Значение по умолчанию неверно.|
| [plot_visible_cells](/cells/ru/python-net/aspose.cells/exporttableoptions/plot_visible_cells) | Экспортирует только видимые ячейки.|
| [plot_visible_rows](/cells/ru/python-net/aspose.cells/exporttableoptions/plot_visible_rows) | Экспортирует только видимые строки.|
| [plot_visible_columns](/cells/ru/python-net/aspose.cells/exporttableoptions/plot_visible_columns) | Экспортирует только видимые столбцы.|
| [export_as_string](/cells/ru/python-net/aspose.cells/exporttableoptions/export_as_string) | Экспортирует строковое значение ячеек в DataTable.|
| [export_as_html_string](/cells/ru/python-net/aspose.cells/exporttableoptions/export_as_html_string) | Экспортирует строковое значение html ячеек в DataTable.|
| [format_strategy](/cells/ru/python-net/aspose.cells/exporttableoptions/format_strategy) | Получает и задает стратегию форматирования при экспорте значения в виде строкового значения.|
| [check_mixed_value_type](/cells/ru/python-net/aspose.cells/exporttableoptions/check_mixed_value_type) |False, Aspose.Cells установит тип DataColumn по типу значения первой строки для повышения производительности.<br/> Правда, Aspose.Cells проверит, смешаны ли типы значений в столбце, прежде чем установить тип DataColumn.<br/> И тип значения смешанный, тип DataColumn будет строковым.|
| [is_vertical](/cells/ru/python-net/aspose.cells/exporttableoptions/is_vertical) | Истинно, если строка в файле рабочей книги представляет строку в DataTable. False, если столбец в файле рабочей книги представляет строку в DataTable.|
| [indexes](/cells/ru/python-net/aspose.cells/exporttableoptions/indexes) |Индексы столбцов/строк, которые необходимо экспортировать.|
| [rename_strategy](/cells/ru/python-net/aspose.cells/exporttableoptions/rename_strategy) | Стратегия дублирования имен столбцов.|



###  Смотрите также
* модуль [aspose.cells](..)
