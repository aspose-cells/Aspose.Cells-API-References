---
title: DataSorter класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 420
url: /ru/python-net/aspose.cells/datasorter/
is_root: false
---
##  DataSorter класс
Краткое описание для DataSorter.



Тип DataSorter предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [keys](/cells/ru/python-net/aspose.cells/datasorter/keys) | Получает список ключей сортировщика данных.|
| [has_headers](/cells/ru/python-net/aspose.cells/datasorter/has_headers) | Указывает, есть ли у диапазона заголовки.|
| [key1](/cells/ru/python-net/aspose.cells/datasorter/key1) | Представляет индекс первого отсортированного столбца (абсолютная позиция, столбец A равен 0, B равен 1,...).|
| [order1](/cells/ru/python-net/aspose.cells/datasorter/order1) | Представляет порядок сортировки первого ключа.|
| [key2](/cells/ru/python-net/aspose.cells/datasorter/key2) | Представляет индекс второго отсортированного столбца (абсолютная позиция, столбец A равен 0, B равен 1, ...).|
| [order2](/cells/ru/python-net/aspose.cells/datasorter/order2) | Представляет порядок сортировки второго ключа.|
| [key3](/cells/ru/python-net/aspose.cells/datasorter/key3) | Представляет индекс третьего отсортированного столбца (абсолютная позиция, столбец A равен 0, B равен 1,...).|
| [order3](/cells/ru/python-net/aspose.cells/datasorter/order3) | Представляет порядок сортировки третьего ключа.|
| [sort_left_to_right](/cells/ru/python-net/aspose.cells/datasorter/sort_left_to_right) | True означает, что сортировка выполняется слева направо.<br/>False означает, что сортировка осуществляется сверху вниз.<br/> Значение по умолчанию неверно.|
| [case_sensitive](/cells/ru/python-net/aspose.cells/datasorter/case_sensitive) | Получает и устанавливает, учитывается ли регистр при сравнении строки.|
| [sort_as_number](/cells/ru/python-net/aspose.cells/datasorter/sort_as_number) | Указывает, сортируется ли что-либо, похожее на число.|


###  Методы
| Метод| Описание|
| :- | :- |
| [add_key(key, order)](/cells/ru/python-net/aspose.cells/datasorter/add_key/#int-SortOrder) | Добавляет отсортированный индекс столбца и порядок сортировки.|
| [add_key(key, order, custom_list)](/cells/ru/python-net/aspose.cells/datasorter/add_key/#int-SortOrder-str) | Добавляет отсортированный индекс столбца и порядок сортировки с пользовательским списком сортировки.|
| [add_key(key, type, order, custom_list)](/cells/ru/python-net/aspose.cells/datasorter/add_key/#int-SortOnType-SortOrder-any) | Добавляет отсортированный индекс столбца и порядок сортировки с пользовательским списком сортировки.|
| [add_key(key, order, custom_list)](/cells/ru/python-net/aspose.cells/datasorter/add_key/#int-SortOrder-list) | Добавляет отсортированный индекс столбца и порядок сортировки с пользовательским списком сортировки.|
| [sort(cells, start_row, start_column, end_row, end_column)](/cells/ru/python-net/aspose.cells/datasorter/sort/#Cells-int-int-int-int) | Сортирует данные области.|
| [sort(cells, area)](/cells/ru/python-net/aspose.cells/datasorter/sort/#Cells-CellArea) | Сортировка данных области.|
| [sort()](/cells/ru/python-net/aspose.cells/datasorter/sort/#) | Отсортируйте данные в диапазоне.|
| [clear()](/cells/ru/python-net/aspose.cells/datasorter/clear/#) | Очистить все настройки.|



###  Пример

```python
from aspose.cells import CellArea, SortOrder, Workbook

# Instantiate a new Workbook object.
workbook = Workbook("Book1.xls")
# Get the workbook datasorter object.
sorter = workbook.data_sorter
# Set the first order for datasorter object.
sorter.order1 = SortOrder.DESCENDING
# Define the first key.
sorter.key1 = 0
# Set the second order for datasorter object.
sorter.order2 = SortOrder.ASCENDING
# Define the second key.
sorter.key2 = 1
# Create a cells area (range).
ca = CellArea()
# Specify the start row index.
ca.start_row = 0
# Specify the start column index.
ca.start_column = 0
# Specify the last row index.
ca.end_row = 13
# Specify the last column index.
ca.end_column = 1
# Sort data in the specified data range (A1:B14)
sorter.sort(workbook.worksheets[0].cells, ca)
# Save the excel file.
workbook.save("outBook.xls")

```

###  Смотрите также
* модуль [aspose.cells](..)
