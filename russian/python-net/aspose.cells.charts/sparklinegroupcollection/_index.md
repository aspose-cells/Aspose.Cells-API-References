---
title: SparklineGroupCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 290
url: /ru/python-net/aspose.cells.charts/sparklinegroupcollection/
is_root: false
---
##  SparklineGroupCollection класс
Инкапсулирует коллекцию из [SparklineGroup](/cells/ru/python-net/aspose.cells.charts/sparklinegroup) объектов.



Тип SparklineGroupCollection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [capacity](/cells/ru/python-net/aspose.cells.charts/sparklinegroupcollection/capacity) | Получает или задает количество элементов, которые может содержать список массивов.|


###  Методы
| Метод| Описание|
| :- | :- |
| [copy_to(array)](/cells/ru/python-net/aspose.cells.charts/sparklinegroupcollection/copy_to/#list) | Копирует весь список массивов в совместимый список одномерных массивов, начиная с начала целевого списка массивов.|
| [copy_to(index, array, array_index, count)](/cells/ru/python-net/aspose.cells.charts/sparklinegroupcollection/copy_to/#int-list-int-int) |Копирует диапазон элементов из списка массивов в совместимый список одномерных массивов, начиная с указанного индекса целевого списка массивов.|
| [index_of(item, index)](/cells/ru/python-net/aspose.cells.charts/sparklinegroupcollection/index_of/#SparklineGroup-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который простирается от указанного индекса до последнего элемента.|
| [index_of(item, index, count)](/cells/ru/python-net/aspose.cells.charts/sparklinegroupcollection/index_of/#SparklineGroup-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который начинается с указанного индекса и содержит указанное количество элементов.|
| [last_index_of(item)](/cells/ru/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения во всем списке массивов.|
| [last_index_of(item, index)](/cells/ru/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который простирается от первого элемента до указанного индекса.|
| [last_index_of(item, index, count)](/cells/ru/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup-int-int) |Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который содержит указанное количество элементов и заканчивается указанным индексом.|
| [add(type, data_range, is_vertical, location_range)](/cells/ru/python-net/aspose.cells.charts/sparklinegroupcollection/add/#SparklineType-str-bool-CellArea) | Добавляет в коллекцию элемент [SparklineGroup](/cells/ru/python-net/aspose.cells.charts/sparklinegroup).|
| [clear_sparklines(cell_area)](/cells/ru/python-net/aspose.cells.charts/sparklinegroupcollection/clear_sparklines/#CellArea) | Очищает спарклайны внутри области ячеек.|
| [clear_sparkline_groups(cell_area)](/cells/ru/python-net/aspose.cells.charts/sparklinegroupcollection/clear_sparkline_groups/#CellArea) | Очищает группы спарклайнов, которые перекрывают область ячеек.|
| [binary_search(item)](/cells/ru/python-net/aspose.cells.charts/sparklinegroupcollection/binary_search/#SparklineGroup) | Ищет элемент во всем отсортированном списке массивов, используя компаратор по умолчанию, и возвращает отсчитываемый от нуля индекс элемента.|



###  Примеры

```python
from aspose.cells import CellArea, SaveFormat, Workbook
from aspose.cells.charts import SparklineType

book = Workbook()
sheet = book.worksheets[0]
sheet.cells.get("A1").put_value(5)
sheet.cells.get("B1").put_value(2)
sheet.cells.get("C1").put_value(1)
sheet.cells.get("D1").put_value(3)
#  Define the CellArea
ca = CellArea()
ca.start_column = 4
ca.end_column = 4
ca.start_row = 0
ca.end_row = 0
idx = sheet.sparkline_group_collection.add(SparklineType.LINE, "A1:D1", False, ca)
group = sheet.sparkline_group_collection[idx]
group.sparkline_collection.add(sheet.name + "!A1:D1", 0, 4)
book.save("output.xlsx", SaveFormat.XLSX)

```

###  Смотрите также
* модуль [aspose.cells.charts](..)
* класс [SparklineGroup](/cells/ru/python-net/aspose.cells.charts/sparklinegroup)
