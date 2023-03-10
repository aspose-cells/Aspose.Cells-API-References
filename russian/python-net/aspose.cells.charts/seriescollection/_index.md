---
title: SeriesCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 240
url: /ru/python-net/aspose.cells.charts/seriescollection/
is_root: false
---
##  SeriesCollection класс
Инкапсулирует коллекцию из [Series](/cells/ru/python-net/aspose.cells.charts/series) объектов.



Тип SeriesCollection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [category_data](/cells/ru/python-net/aspose.cells.charts/seriescollection/category_data) | Получает или задает диапазон значений оси категории.<br/> Это может быть диапазон ячеек (например, «d1:e10»),<br/> или последовательность значений (например, "{2,6,8,10}").|
| [second_category_data](/cells/ru/python-net/aspose.cells.charts/seriescollection/second_category_data) | Получает или задает диапазон значений оси второй категории.<br/> Это может быть диапазон ячеек (например, «d1:e10»),<br/> или последовательность значений (например, "{2,6,8,10}").<br/> Воздействует только тогда, когда некоторые ASeries строятся по второй оси.|
| [is_color_varied](/cells/ru/python-net/aspose.cells.charts/seriescollection/is_color_varied) | Представляет, если цвет точек различен.|
| [capacity](/cells/ru/python-net/aspose.cells.charts/seriescollection/capacity) | Получает или задает количество элементов, которые может содержать список массивов.|


###  Методы
| Метод| Описание|
| :- | :- |
| [add(area, is_vertical)](/cells/ru/python-net/aspose.cells.charts/seriescollection/add/#str-bool) | Добавляет коллекцию [SeriesCollection](/cells/ru/python-net/aspose.cells.charts/seriescollection) на диаграмму.|
| [add(area, is_vertical, check_labels)](/cells/ru/python-net/aspose.cells.charts/seriescollection/add/#str-bool-bool) | Добавляет коллекцию [SeriesCollection](/cells/ru/python-net/aspose.cells.charts/seriescollection) на диаграмму.|
| [copy_to(array)](/cells/ru/python-net/aspose.cells.charts/seriescollection/copy_to/#list) | Копирует весь список массивов в совместимый список одномерных массивов, начиная с начала целевого списка массивов.|
| [copy_to(index, array, array_index, count)](/cells/ru/python-net/aspose.cells.charts/seriescollection/copy_to/#int-list-int-int) |Копирует диапазон элементов из списка массивов в совместимый список одномерных массивов, начиная с указанного индекса целевого списка массивов.|
| [index_of(item, index)](/cells/ru/python-net/aspose.cells.charts/seriescollection/index_of/#Series-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который простирается от указанного индекса до последнего элемента.|
| [index_of(item, index, count)](/cells/ru/python-net/aspose.cells.charts/seriescollection/index_of/#Series-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который начинается с указанного индекса и содержит указанное количество элементов.|
| [last_index_of(item)](/cells/ru/python-net/aspose.cells.charts/seriescollection/last_index_of/#Series) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения во всем списке массивов.|
| [last_index_of(item, index)](/cells/ru/python-net/aspose.cells.charts/seriescollection/last_index_of/#Series-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который простирается от первого элемента до указанного индекса.|
| [last_index_of(item, index, count)](/cells/ru/python-net/aspose.cells.charts/seriescollection/last_index_of/#Series-int-int) |Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который содержит указанное количество элементов и заканчивается указанным индексом.|
| [get_series_by_order(order)](/cells/ru/python-net/aspose.cells.charts/seriescollection/get_series_by_order/#int) | Получает элемент [Series](/cells/ru/python-net/aspose.cells.charts/series) по порядку.|
| [change_series_order(source_index, dest_index)](/cells/ru/python-net/aspose.cells.charts/seriescollection/change_series_order/#int-int) | Напрямую меняет порядок двух серий.|
| [set_series_names(start_index, area, is_vertical)](/cells/ru/python-net/aspose.cells.charts/seriescollection/set_series_names/#int-str-bool) | Задает имя всех рядов на диаграмме.|
| [add_r1c1(area, is_vertical)](/cells/ru/python-net/aspose.cells.charts/seriescollection/add_r1c1/#str-bool) | Добавляет коллекцию [SeriesCollection](/cells/ru/python-net/aspose.cells.charts/seriescollection) на диаграмму.|
| [binary_search(item)](/cells/ru/python-net/aspose.cells.charts/seriescollection/binary_search/#Series) | Ищет элемент во всем отсортированном списке массивов, используя компаратор по умолчанию, и возвращает отсчитываемый от нуля индекс элемента.|



###  Пример

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Excel object
sheetIndex = workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[sheetIndex]
# Adding a sample value to "A1" cell
worksheet.cells.get("A1").put_value(50)
# Adding a sample value to "A2" cell
worksheet.cells.get("A2").put_value(100)
# Adding a sample value to "A3" cell
worksheet.cells.get("A3").put_value(150)
# Adding a sample value to "A4" cell
worksheet.cells.get("A4").put_value(200)
# Adding a sample value to "B1" cell
worksheet.cells.get("B1").put_value(60)
# Adding a sample value to "B2" cell
worksheet.cells.get("B2").put_value(32)
# Adding a sample value to "B3" cell
worksheet.cells.get("B3").put_value(50)
# Adding a sample value to "B4" cell
worksheet.cells.get("B4").put_value(40)
# Adding a sample value to "C1" cell as category data
worksheet.cells.get("C1").put_value("Q1")
# Adding a sample value to "C2" cell as category data
worksheet.cells.get("C2").put_value("Q2")
# Adding a sample value to "C3" cell as category data
worksheet.cells.get("C3").put_value("Y1")
# Adding a sample value to "C4" cell as category data
worksheet.cells.get("C4").put_value("Y2")
# Adding a chart to the worksheet
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 15, 5)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.n_series.add("A1:B4", True)
# Setting the data source for the category data of NSeries
chart.n_series.category_data = "C1:C4"
# Saving the Excel file
workbook.save("book1.xls")

```

###  Смотрите также
* модуль [aspose.cells.charts](..)
* класс [Series](/cells/ru/python-net/aspose.cells.charts/series)
* класс [SeriesCollection](/cells/ru/python-net/aspose.cells.charts/seriescollection)
