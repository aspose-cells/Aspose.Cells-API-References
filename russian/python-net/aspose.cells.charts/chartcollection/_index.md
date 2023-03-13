---
title: ChartCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 50
url: /ru/python-net/aspose.cells.charts/chartcollection/
is_root: false
---
##  ChartCollection класс
Инкапсулирует коллекцию из [Chart](/cells/ru/python-net/aspose.cells.charts/chart) объектов.



Тип ChartCollection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [capacity](/cells/ru/python-net/aspose.cells.charts/chartcollection/capacity) | Получает или задает количество элементов, которые может содержать список массивов.|


###  Методы
| Метод| Описание|
| :- | :- |
| [add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column)](/cells/ru/python-net/aspose.cells.charts/chartcollection/add/#ChartType-int-int-int-int) | Добавляет диаграмму в коллекцию.|
| [add(type, data_range, top_row, left_column, right_row, bottom_column)](/cells/ru/python-net/aspose.cells.charts/chartcollection/add/#ChartType-str-int-int-int-int) | Добавляет диаграмму в коллекцию.|
| [add(data, data_range, is_vertical, top_row, left_column, right_row, bottom_column)](/cells/ru/python-net/aspose.cells.charts/chartcollection/add/#bytes-str-bool-int-int-int-int) | Добавляет диаграмму с предустановленным шаблоном.|
| [add(type, data_range, is_vertical, top_row, left_column, right_row, bottom_column)](/cells/ru/python-net/aspose.cells.charts/chartcollection/add/#ChartType-str-bool-int-int-int-int) | Добавляет диаграмму в коллекцию.|
| [get(index)](/cells/ru/python-net/aspose.cells.charts/chartcollection/get/#int) |Добавить API for Python через .Net.так как это [индекс int] не поддерживается|
| [get(name)](/cells/ru/python-net/aspose.cells.charts/chartcollection/get/#str) | Добавить API for Python через .Net.так как это [string Chart] не поддерживается|
| [copy_to(array)](/cells/ru/python-net/aspose.cells.charts/chartcollection/copy_to/#list) | Копирует весь список массивов в совместимый список одномерных массивов, начиная с начала целевого списка массивов.|
| [copy_to(index, array, array_index, count)](/cells/ru/python-net/aspose.cells.charts/chartcollection/copy_to/#int-list-int-int) |Копирует диапазон элементов из списка массивов в совместимый список одномерных массивов, начиная с указанного индекса целевого списка массивов.|
| [index_of(item, index)](/cells/ru/python-net/aspose.cells.charts/chartcollection/index_of/#Chart-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который простирается от указанного индекса до последнего элемента.|
| [index_of(item, index, count)](/cells/ru/python-net/aspose.cells.charts/chartcollection/index_of/#Chart-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который начинается с указанного индекса и содержит указанное количество элементов.|
| [last_index_of(item)](/cells/ru/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения во всем списке массивов.|
| [last_index_of(item, index)](/cells/ru/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который простирается от первого элемента до указанного индекса.|
| [last_index_of(item, index, count)](/cells/ru/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart-int-int) |Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который содержит указанное количество элементов и заканчивается указанным индексом.|
| [add_floating_chart(type, left, top, width, height)](/cells/ru/python-net/aspose.cells.charts/chartcollection/add_floating_chart/#ChartType-int-int-int-int) | Добавляет диаграмму в коллекцию.|
| [binary_search(item)](/cells/ru/python-net/aspose.cells.charts/chartcollection/binary_search/#Chart) | Ищет элемент во всем отсортированном списке массивов, используя компаратор по умолчанию, и возвращает отсчитываемый от нуля индекс элемента.|



###  Пример

```python
from aspose.cells import Workbook

workbook = Workbook()
charts = workbook.worksheets[0].charts

```

###  Смотрите также
* модуль [aspose.cells.charts](..)
* класс [Chart](/cells/ru/python-net/aspose.cells.charts/chart)
