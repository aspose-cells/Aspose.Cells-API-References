---
title: HyperlinkCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 800
url: /ru/python-net/aspose.cells/hyperlinkcollection/
is_root: false
---
##  HyperlinkCollection класс
Инкапсулирует коллекцию из [Hyperlink](/cells/ru/python-net/aspose.cells/hyperlink) объектов.



Тип HyperlinkCollection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [capacity](/cells/ru/python-net/aspose.cells/hyperlinkcollection/capacity) | Получает или задает количество элементов, которые может содержать список массивов.|


###  Методы
| Метод| Описание|
| :- | :- |
| [add(first_row, first_column, total_rows, total_columns, address)](/cells/ru/python-net/aspose.cells/hyperlinkcollection/add/#int-int-int-int-str) | Добавляет гиперссылку к указанной ячейке или диапазону ячеек.|
| [add(cell_name, total_rows, total_columns, address)](/cells/ru/python-net/aspose.cells/hyperlinkcollection/add/#str-int-int-str) | Добавляет гиперссылку к указанной ячейке или диапазону ячеек.|
| [add(start_cell_name, end_cell_name, address, text_to_display, screen_tip)](/cells/ru/python-net/aspose.cells/hyperlinkcollection/add/#str-str-str-str-str) | Добавляет гиперссылку к указанной ячейке или диапазону ячеек.|
| [copy_to(array)](/cells/ru/python-net/aspose.cells/hyperlinkcollection/copy_to/#list) | Копирует весь список массивов в совместимый список одномерных массивов, начиная с начала целевого списка массивов.|
| [copy_to(index, array, array_index, count)](/cells/ru/python-net/aspose.cells/hyperlinkcollection/copy_to/#int-list-int-int) | Копирует диапазон элементов из списка массивов в совместимый список одномерных массивов, начиная с указанного индекса целевого списка массивов.|
| [index_of(item, index)](/cells/ru/python-net/aspose.cells/hyperlinkcollection/index_of/#Hyperlink-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который простирается от указанного индекса до последнего элемента.|
| [index_of(item, index, count)](/cells/ru/python-net/aspose.cells/hyperlinkcollection/index_of/#Hyperlink-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который начинается с указанного индекса и содержит указанное количество элементов.|
| [last_index_of(item)](/cells/ru/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения во всем списке массивов.|
| [last_index_of(item, index)](/cells/ru/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink-int) |Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который простирается от первого элемента до указанного индекса.|
| [last_index_of(item, index, count)](/cells/ru/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который содержит указанное количество элементов и заканчивается указанным индексом.|
| [binary_search(item)](/cells/ru/python-net/aspose.cells/hyperlinkcollection/binary_search/#Hyperlink) | Ищет элемент во всем отсортированном списке массивов, используя компаратор по умолчанию, и возвращает отсчитываемый от нуля индекс элемента.|



###  Пример

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Get Hyperlinks Collection
hyperlinks = worksheet.hyperlinks
# Adding a hyperlink to a URL at "A1" cell
hyperlinks.add("A1", 1, 1, "http://www.aspose.com")
# Saving the Excel file
workbook.save("book1.xls")

```

###  Смотрите также
* модуль [aspose.cells](..)
* класс [Hyperlink](/cells/ru/python-net/aspose.cells/hyperlink)
