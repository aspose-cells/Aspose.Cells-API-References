---
title: TimelineCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells.timelines/timelinecollection/
is_root: false
---
##  TimelineCollection класс
Задает коллекцию всех объектов временной шкалы на указанном листе.
Из-за MS Excel Excel 2003 не поддерживает временную шкалу.



Тип TimelineCollection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [capacity](/cells/ru/python-net/aspose.cells.timelines/timelinecollection/capacity) | Получает или задает количество элементов, которые может содержать список массивов.|


###  Методы
| Метод| Описание|
| :- | :- |
| [add(pivot, row, column, base_field_name)](/cells/ru/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-int-int-str) | Добавьте новую временную шкалу, используя сводную таблицу в качестве источника данных.|
| [add(pivot, dest_cell_name, base_field_name)](/cells/ru/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-str-str) | Добавьте новую временную шкалу, используя сводную таблицу в качестве источника данных.|
| [add(pivot, row, column, base_field_index)](/cells/ru/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-int-int-int) | Добавьте новую временную шкалу, используя сводную таблицу в качестве источника данных.|
| [add(pivot, dest_cell_name, base_field_index)](/cells/ru/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-str-int) | Добавьте новую временную шкалу, используя сводную таблицу в качестве источника данных.|
| [add(pivot, row, column, base_field)](/cells/ru/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField) | Добавьте новую временную шкалу, используя сводную таблицу в качестве источника данных.|
| [add(pivot, dest_cell_name, base_field)](/cells/ru/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField) | Добавьте новую временную шкалу, используя сводную таблицу в качестве источника данных.|
| [copy_to(array)](/cells/ru/python-net/aspose.cells.timelines/timelinecollection/copy_to/#list) | Копирует весь список массивов в совместимый список одномерных массивов, начиная с начала целевого списка массивов.|
| [copy_to(index, array, array_index, count)](/cells/ru/python-net/aspose.cells.timelines/timelinecollection/copy_to/#int-list-int-int) |Копирует диапазон элементов из списка массивов в совместимый список одномерных массивов, начиная с указанного индекса целевого списка массивов.|
| [index_of(item, index)](/cells/ru/python-net/aspose.cells.timelines/timelinecollection/index_of/#Timeline-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который простирается от указанного индекса до последнего элемента.|
| [index_of(item, index, count)](/cells/ru/python-net/aspose.cells.timelines/timelinecollection/index_of/#Timeline-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который начинается с указанного индекса и содержит указанное количество элементов.|
| [last_index_of(item)](/cells/ru/python-net/aspose.cells.timelines/timelinecollection/last_index_of/#Timeline) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения во всем списке массивов.|
| [last_index_of(item, index)](/cells/ru/python-net/aspose.cells.timelines/timelinecollection/last_index_of/#Timeline-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который простирается от первого элемента до указанного индекса.|
| [last_index_of(item, index, count)](/cells/ru/python-net/aspose.cells.timelines/timelinecollection/last_index_of/#Timeline-int-int) |Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который содержит указанное количество элементов и заканчивается указанным индексом.|
| [binary_search(item)](/cells/ru/python-net/aspose.cells.timelines/timelinecollection/binary_search/#Timeline) | Ищет элемент во всем отсортированном списке массивов, используя компаратор по умолчанию, и возвращает отсчитываемый от нуля индекс элемента.|



###  Примеры

```python
from aspose.cells import CellsFactory, Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType
import datetime

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
# Create date style
dateStyle = CellsFactory().create_style()
dateStyle.custom = "m/d/yyyy"
cells.get(0, 1).value = "date"
cells.get(1, 1).value = datetime(2021, 2, 5)
cells.get(2, 1).value = datetime(2022, 3, 8)
cells.get(3, 1).value = datetime(2023, 4, 10)
cells.get(4, 1).value = datetime(2024, 5, 16)
# Set date style
cells.get(1, 1).set_style(dateStyle)
cells.get(2, 1).set_style(dateStyle)
cells.get(3, 1).set_style(dateStyle)
cells.get(4, 1).set_style(dateStyle)
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
pivots = sheet.pivot_tables
# Add a PivotTable
pivotIndex = pivots.add("=Sheet1!A1:C5", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "date")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Refresh PivotTable data
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  Смотрите также
* модуль [aspose.cells.timelines](..)
