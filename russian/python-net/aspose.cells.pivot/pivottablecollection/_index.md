---
title: PivotTableCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 110
url: /ru/python-net/aspose.cells.pivot/pivottablecollection/
is_root: false
---
##  PivotTableCollection класс
Представляет коллекцию всех объектов сводной таблицы на указанном листе.



Тип PivotTableCollection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [capacity](/cells/ru/python-net/aspose.cells.pivot/pivottablecollection/capacity) | Получает или задает количество элементов, которые может содержать список массивов.|


###  Методы
| Метод| Описание|
| :- | :- |
| [add(source_data, dest_cell_name, table_name)](/cells/ru/python-net/aspose.cells.pivot/pivottablecollection/add/#str-str-str) | Добавляет новый кэш сводной таблицы в коллекцию сводных кешей.|
| [add(source_data, dest_cell_name, table_name, use_same_source)](/cells/ru/python-net/aspose.cells.pivot/pivottablecollection/add/#str-str-str-bool) | Добавляет новый кэш сводной таблицы в коллекцию сводных кешей.|
| [add(source_data, row, column, table_name)](/cells/ru/python-net/aspose.cells.pivot/pivottablecollection/add/#str-int-int-str) | Добавляет новый кэш сводной таблицы в коллекцию сводных кешей.|
| [add(source_data, row, column, table_name, use_same_source)](/cells/ru/python-net/aspose.cells.pivot/pivottablecollection/add/#str-int-int-str-bool) | Добавляет новый кэш сводной таблицы в коллекцию сводных кешей.|
| [add(pivot_table, dest_cell_name, table_name)](/cells/ru/python-net/aspose.cells.pivot/pivottablecollection/add/#PivotTable-str-str) | Добавляет новый объект сводной таблицы в коллекцию из другой сводной таблицы.|
| [add(pivot_table, row, column, table_name)](/cells/ru/python-net/aspose.cells.pivot/pivottablecollection/add/#PivotTable-int-int-str) | Добавляет новый объект сводной таблицы в коллекцию из другой сводной таблицы.|
| [add(source_data, is_auto_page, page_fields, dest_cell_name, table_name)](/cells/ru/python-net/aspose.cells.pivot/pivottablecollection/add/#list-bool-PivotPageFields-str-str) | Добавляет новый объект сводной таблицы в коллекцию с несколькими диапазонами консолидации в качестве источника данных.|
| [add(source_data, is_auto_page, page_fields, row, column, table_name)](/cells/ru/python-net/aspose.cells.pivot/pivottablecollection/add/#list-bool-PivotPageFields-int-int-str) | Добавляет новый объект сводной таблицы в коллекцию с несколькими диапазонами консолидации в качестве источника данных.|
| [copy_to(array)](/cells/ru/python-net/aspose.cells.pivot/pivottablecollection/copy_to/#list) | Копирует весь список массивов в совместимый список одномерных массивов, начиная с начала целевого списка массивов.|
| [copy_to(index, array, array_index, count)](/cells/ru/python-net/aspose.cells.pivot/pivottablecollection/copy_to/#int-list-int-int) |Копирует диапазон элементов из списка массивов в совместимый список одномерных массивов, начиная с указанного индекса целевого списка массивов.|
| [index_of(item, index)](/cells/ru/python-net/aspose.cells.pivot/pivottablecollection/index_of/#PivotTable-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который простирается от указанного индекса до последнего элемента.|
| [index_of(item, index, count)](/cells/ru/python-net/aspose.cells.pivot/pivottablecollection/index_of/#PivotTable-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который начинается с указанного индекса и содержит указанное количество элементов.|
| [last_index_of(item)](/cells/ru/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#PivotTable) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения во всем списке массивов.|
| [last_index_of(item, index)](/cells/ru/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#PivotTable-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который простирается от первого элемента до указанного индекса.|
| [last_index_of(item, index, count)](/cells/ru/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#PivotTable-int-int) |Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который содержит указанное количество элементов и заканчивается указанным индексом.|
| [remove_at(index, keep_data)](/cells/ru/python-net/aspose.cells.pivot/pivottablecollection/remove_at/#int-bool) | Удаляет сводную таблицу по указанному индексу.|
| [binary_search(item)](/cells/ru/python-net/aspose.cells.pivot/pivottablecollection/binary_search/#PivotTable) | Ищет элемент во всем отсортированном списке массивов, используя компаратор по умолчанию, и возвращает отсчитываемый от нуля индекс элемента.|



###  Примеры

```python
from aspose.cells import FormatConditionType, OperatorType, Workbook
from aspose.cells.pivot import PivotFieldType, PivotFilterType, PivotTableStyleType
from aspose.pydrawing import Color

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Change PivotField's attributes
rowField = pivot.row_fields[0]
rowField.display_name = "custom display name"
# Add PivotFilter
index = pivot.pivot_filters.add(0, PivotFilterType.COUNT)
filter = pivot.pivot_filters[index]
filter.auto_filter.filter_top10(0, False, False, 2)
# Add PivotFormatCondition
formatIndex = pivot.pivot_format_conditions.add()
pfc = pivot.pivot_format_conditions[formatIndex]
fcc = pfc.format_conditions
fcc.add_area(pivot.data_body_range)
idx = fcc.add_condition(FormatConditionType.CELL_VALUE)
fc = fcc[idx]
fc.formula1 = "100"
fc.operator = OperatorType.GREATER_OR_EQUAL
fc.style.background_color = Color.red
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  Смотрите также
* модуль [aspose.cells.pivot](..)
