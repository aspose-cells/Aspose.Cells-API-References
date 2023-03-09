---
title: ListObject класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 30
url: /ru/python-net/aspose.cells.tables/listobject/
is_root: false
---
##  ListObject класс
Представляет объект списка на листе.
 Объект ListObject является членом коллекции ListObjects.
Коллекция ListObjects содержит все объекты списка на листе.



Тип ListObject предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [start_row](/cells/ru/python-net/aspose.cells.tables/listobject/start_row) | Получает начальную строку диапазона.|
| [start_column](/cells/ru/python-net/aspose.cells.tables/listobject/start_column) | Получает начальный столбец диапазона.|
| [end_row](/cells/ru/python-net/aspose.cells.tables/listobject/end_row) | Получает конечную строку диапазона.|
| [end_column](/cells/ru/python-net/aspose.cells.tables/listobject/end_column) |Получает конечный столбец диапазона.|
| [list_columns](/cells/ru/python-net/aspose.cells.tables/listobject/list_columns) | Получает ListColumns объекта ListObject.|
| [show_header_row](/cells/ru/python-net/aspose.cells.tables/listobject/show_header_row) | Получает и устанавливает, показывает ли этот ListObject строку заголовка.|
| [show_totals](/cells/ru/python-net/aspose.cells.tables/listobject/show_totals) | Получает и устанавливает, показывает ли этот ListObject общее количество строк.|
| [data_range](/cells/ru/python-net/aspose.cells.tables/listobject/data_range) | Получает диапазон данных ListObject.|
| [query_table](/cells/ru/python-net/aspose.cells.tables/listobject/query_table) | Получает связанную таблицу запросов.|
| [data_source_type](/cells/ru/python-net/aspose.cells.tables/listobject/data_source_type) | Получает тип источника данных таблицы.|
| [auto_filter](/cells/ru/python-net/aspose.cells.tables/listobject/auto_filter) | Получает автоматический фильтр.|
| [display_name](/cells/ru/python-net/aspose.cells.tables/listobject/display_name) | Получает и задает отображаемое имя.|
| [comment](/cells/ru/python-net/aspose.cells.tables/listobject/comment) | Получает и задает комментарий к таблице.|
| [show_table_style_first_column](/cells/ru/python-net/aspose.cells.tables/listobject/show_table_style_first_column) | Указывает, следует ли применять стиль к первому столбцу в таблице.|
| [show_table_style_last_column](/cells/ru/python-net/aspose.cells.tables/listobject/show_table_style_last_column) | Указывает, следует ли применять стиль к последнему столбцу в таблице.|
| [show_table_style_row_stripes](/cells/ru/python-net/aspose.cells.tables/listobject/show_table_style_row_stripes) | Указывает, применяется ли форматирование чередования строк.|
| [show_table_style_column_stripes](/cells/ru/python-net/aspose.cells.tables/listobject/show_table_style_column_stripes) | Указывает, применяется ли форматирование чередования столбцов.|
| [table_style_type](/cells/ru/python-net/aspose.cells.tables/listobject/table_style_type) | Gets и встроенный стиль таблицы.|
| [table_style_name](/cells/ru/python-net/aspose.cells.tables/listobject/table_style_name) | Получает и задает имя стиля таблицы.|
| [xml_map](/cells/ru/python-net/aspose.cells.tables/listobject/xml_map) | Получает [ListObject.xml_map](/cells/ru/python-net/aspose.cells.tables/listobject#xml_map), используемый для этого списка.|
| [alternative_text](/cells/ru/python-net/aspose.cells.tables/listobject/alternative_text) | Получает и задает альтернативный текст.|
| [alternative_description](/cells/ru/python-net/aspose.cells.tables/listobject/alternative_description) | Получает и задает альтернативное описание.|


###  Методы
| Метод| Описание|
| :- | :- |
| [convert_to_range()](/cells/ru/python-net/aspose.cells.tables/listobject/convert_to_range/#) | Преобразуйте таблицу в диапазон.|
| [convert_to_range(options)](/cells/ru/python-net/aspose.cells.tables/listobject/convert_to_range/#TableToRangeOptions) | Преобразуйте таблицу в диапазон.|
| [resize(start_row, start_column, end_row, end_column, has_headers)](/cells/ru/python-net/aspose.cells.tables/listobject/resize/#int-int-int-int-bool) | Измените размер диапазона объекта списка.|
| [put_cell_value(row_offset, column_offset, value)](/cells/ru/python-net/aspose.cells.tables/listobject/put_cell_value/#int-int-any) | Поместите значение в ячейку.|
| [update_column_name()](/cells/ru/python-net/aspose.cells.tables/listobject/update_column_name/#) |Обновляет имена всех столбцов списка на листе.|
| [filter()](/cells/ru/python-net/aspose.cells.tables/listobject/filter/#) | Отфильтруйте таблицу.|
| [apply_style_to_range()](/cells/ru/python-net/aspose.cells.tables/listobject/apply_style_to_range/#) | Примените стиль таблицы к диапазону.|



###  Примеры

```python
from aspose.cells import CellsHelper, Workbook
from aspose.cells.tables import TotalsCalculation

workbook = Workbook()
cells = workbook.worksheets[0].cells
for i in range(5):
    cells.get(0, i).put_value(CellsHelper.column_index_to_name(i))
for row in range(1, 10):
    for column in range(5):
        cells.get(row, column).put_value(row * column)
tables = workbook.worksheets[0].list_objects
index = tables.add(0, 0, 9, 4, True)
table = tables[0]
table.show_totals = True
table.list_columns[4].totals_calculation = TotalsCalculation.SUM
workbook.save(r"Book1.xlsx")

```

###  Смотрите также
* модуль [aspose.cells.tables](..)
