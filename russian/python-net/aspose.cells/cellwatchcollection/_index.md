---
title: CellWatchCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 170
url: /ru/python-net/aspose.cells/cellwatchcollection/
is_root: false
---
##  CellWatchCollection класс
Представляет набор ячеек на этом рабочем листе, за которым наблюдают в «окне просмотра».



Тип CellWatchCollection предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [CellWatchCollection()](/cells/ru/python-net/aspose.cells/cellwatchcollection/__init__/#) |Создает новый экземпляр CellWatchCollection|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [capacity](/cells/ru/python-net/aspose.cells/cellwatchcollection/capacity) | Получает или задает количество элементов, которые может содержать список массивов.|


###  Методы
| Метод| Описание|
| :- | :- |
| [add(row, column)](/cells/ru/python-net/aspose.cells/cellwatchcollection/add/#int-int) | Добавляет [CellWatch](/cells/ru/python-net/aspose.cells/cellwatch) со строкой и столбцом.|
| [add(cell_name)](/cells/ru/python-net/aspose.cells/cellwatchcollection/add/#str) | Добавляет [CellWatch](/cells/ru/python-net/aspose.cells/cellwatch) с названием ячейки.|
| [copy_to(array)](/cells/ru/python-net/aspose.cells/cellwatchcollection/copy_to/#list) | Копирует весь список массивов в совместимый список одномерных массивов, начиная с начала целевого списка массивов.|
| [copy_to(index, array, array_index, count)](/cells/ru/python-net/aspose.cells/cellwatchcollection/copy_to/#int-list-int-int) | Копирует диапазон элементов из списка массивов в совместимый список одномерных массивов, начиная с указанного индекса целевого списка массивов.|
| [index_of(item, index)](/cells/ru/python-net/aspose.cells/cellwatchcollection/index_of/#CellWatch-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который простирается от указанного индекса до последнего элемента.|
| [index_of(item, index, count)](/cells/ru/python-net/aspose.cells/cellwatchcollection/index_of/#CellWatch-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который начинается с указанного индекса и содержит указанное количество элементов.|
| [last_index_of(item)](/cells/ru/python-net/aspose.cells/cellwatchcollection/last_index_of/#CellWatch) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения во всем списке массивов.|
| [last_index_of(item, index)](/cells/ru/python-net/aspose.cells/cellwatchcollection/last_index_of/#CellWatch-int) |Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который простирается от первого элемента до указанного индекса.|
| [last_index_of(item, index, count)](/cells/ru/python-net/aspose.cells/cellwatchcollection/last_index_of/#CellWatch-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который содержит указанное количество элементов и заканчивается указанным индексом.|
| [binary_search(item)](/cells/ru/python-net/aspose.cells/cellwatchcollection/binary_search/#CellWatch) | Ищет элемент во всем отсортированном списке массивов, используя компаратор по умолчанию, и возвращает отсчитываемый от нуля индекс элемента.|



###  Пример

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet.
sheet = workbook.worksheets[0]
#  Add Cell Watch Item into the watch window
sheet.cell_watches.add("B2")

```

###  Смотрите также
* модуль [aspose.cells](..)
* класс [CellWatch](/cells/ru/python-net/aspose.cells/cellwatch)
