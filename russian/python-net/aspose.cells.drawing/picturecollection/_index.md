---
title: PictureCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 460
url: /ru/python-net/aspose.cells.drawing/picturecollection/
is_root: false
---
##  PictureCollection класс
Инкапсулирует коллекцию из [Picture](/cells/ru/python-net/aspose.cells.drawing/picture) объектов.



Тип PictureCollection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [capacity](/cells/ru/python-net/aspose.cells.drawing/picturecollection/capacity) | Получает или задает количество элементов, которые может содержать список массивов.|


###  Методы
| Метод| Описание|
| :- | :- |
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)](/cells/ru/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-io.RawIOBase) | Добавляет изображение в коллекцию.|
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name)](/cells/ru/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-str) | Добавляет изображение в коллекцию.|
| [add(upper_left_row, upper_left_column, stream)](/cells/ru/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase) | Добавляет изображение в коллекцию.|
| [add(upper_left_row, upper_left_column, file_name)](/cells/ru/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str) | Добавляет изображение в коллекцию.|
| [add(upper_left_row, upper_left_column, stream, width_scale, height_scale)](/cells/ru/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase-int-int) | Добавляет изображение в коллекцию.|
| [add(upper_left_row, upper_left_column, file_name, width_scale, height_scale)](/cells/ru/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str-int-int) | Добавляет изображение в коллекцию.|
| [copy_to(array)](/cells/ru/python-net/aspose.cells.drawing/picturecollection/copy_to/#list) | Копирует весь список массивов в совместимый список одномерных массивов, начиная с начала целевого списка массивов.|
| [copy_to(index, array, array_index, count)](/cells/ru/python-net/aspose.cells.drawing/picturecollection/copy_to/#int-list-int-int) |Копирует диапазон элементов из списка массивов в совместимый список одномерных массивов, начиная с указанного индекса целевого списка массивов.|
| [index_of(item, index)](/cells/ru/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который простирается от указанного индекса до последнего элемента.|
| [index_of(item, index, count)](/cells/ru/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который начинается с указанного индекса и содержит указанное количество элементов.|
| [last_index_of(item)](/cells/ru/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения во всем списке массивов.|
| [last_index_of(item, index)](/cells/ru/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который простирается от первого элемента до указанного индекса.|
| [last_index_of(item, index, count)](/cells/ru/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int-int) |Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который содержит указанное количество элементов и заканчивается указанным индексом.|
| [binary_search(item)](/cells/ru/python-net/aspose.cells.drawing/picturecollection/binary_search/#Picture) | Ищет элемент во всем отсортированном списке массивов, используя компаратор по умолчанию, и возвращает отсчитываемый от нуля индекс элемента.|



###  Примеры

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# get PictureCollection
pictures = workbook.worksheets[0].pictures
# do your business
# Save the excel file.
workbook.save("result.xlsx")

```

###  Смотрите также
* модуль [aspose.cells.drawing](..)
* класс [Picture](/cells/ru/python-net/aspose.cells.drawing/picture)
