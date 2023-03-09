---
title: HorizontalPageBreakCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 760
url: /ru/python-net/aspose.cells/horizontalpagebreakcollection/
is_root: false
---
##  HorizontalPageBreakCollection класс
Инкапсулирует коллекцию из [HorizontalPageBreak](/cells/ru/python-net/aspose.cells/horizontalpagebreak) объектов.



Тип HorizontalPageBreakCollection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [capacity](/cells/ru/python-net/aspose.cells/horizontalpagebreakcollection/capacity) | Получает или задает количество элементов, которые может содержать список массивов.|


###  Методы
| Метод| Описание|
| :- | :- |
| [add(row, start_column, end_column)](/cells/ru/python-net/aspose.cells/horizontalpagebreakcollection/add/#int-int-int) | Добавляет в коллекцию горизонтальный разрыв страницы.|
| [add(row)](/cells/ru/python-net/aspose.cells/horizontalpagebreakcollection/add/#int) | Добавляет в коллекцию горизонтальный разрыв страницы.|
| [add(row, column)](/cells/ru/python-net/aspose.cells/horizontalpagebreakcollection/add/#int-int) | Добавляет в коллекцию горизонтальный разрыв страницы.|
| [add(cell_name)](/cells/ru/python-net/aspose.cells/horizontalpagebreakcollection/add/#str) | Добавляет в коллекцию горизонтальный разрыв страницы.|
| [copy_to(array)](/cells/ru/python-net/aspose.cells/horizontalpagebreakcollection/copy_to/#list) | Копирует весь список массивов в совместимый список одномерных массивов, начиная с начала целевого списка массивов.|
| [copy_to(index, array, array_index, count)](/cells/ru/python-net/aspose.cells/horizontalpagebreakcollection/copy_to/#int-list-int-int) |Копирует диапазон элементов из списка массивов в совместимый список одномерных массивов, начиная с указанного индекса целевого списка массивов.|
| [index_of(item, index)](/cells/ru/python-net/aspose.cells/horizontalpagebreakcollection/index_of/#HorizontalPageBreak-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который простирается от указанного индекса до последнего элемента.|
| [index_of(item, index, count)](/cells/ru/python-net/aspose.cells/horizontalpagebreakcollection/index_of/#HorizontalPageBreak-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который начинается с указанного индекса и содержит указанное количество элементов.|
| [last_index_of(item)](/cells/ru/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения во всем списке массивов.|
| [last_index_of(item, index)](/cells/ru/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который простирается от первого элемента до указанного индекса.|
| [last_index_of(item, index, count)](/cells/ru/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak-int-int) |Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который содержит указанное количество элементов и заканчивается указанным индексом.|
| [binary_search(item)](/cells/ru/python-net/aspose.cells/horizontalpagebreakcollection/binary_search/#HorizontalPageBreak) | Ищет элемент во всем отсортированном списке массивов, используя компаратор по умолчанию, и возвращает отсчитываемый от нуля индекс элемента.|



###  Примеры

```python
from aspose.cells import Workbook

excel = Workbook()
# Add a pagebreak at G5
excel.worksheets[0].horizontal_page_breaks.add("G5")
excel.worksheets[0].vertical_page_breaks.add("G5")

```

###  Смотрите также
* модуль [aspose.cells](..)
* класс [HorizontalPageBreak](/cells/ru/python-net/aspose.cells/horizontalpagebreak)
