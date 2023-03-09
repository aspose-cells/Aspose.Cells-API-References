---
title: ValidationCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 1550
url: /ru/python-net/aspose.cells/validationcollection/
is_root: false
---
##  ValidationCollection класс
Представляет коллекцию проверки данных.



Тип ValidationCollection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [capacity](/cells/ru/python-net/aspose.cells/validationcollection/capacity) | Получает или задает количество элементов, которые может содержать список массивов.|


###  Методы
| Метод| Описание|
| :- | :- |
| [add()](/cells/ru/python-net/aspose.cells/validationcollection/add/#) | Добавляет проверку данных в коллекцию.|
| [add(ca)](/cells/ru/python-net/aspose.cells/validationcollection/add/#CellArea) | Добавляет проверку данных в коллекцию.|
| [copy_to(array)](/cells/ru/python-net/aspose.cells/validationcollection/copy_to/#list) | Копирует весь список массивов в совместимый список одномерных массивов, начиная с начала целевого списка массивов.|
| [copy_to(index, array, array_index, count)](/cells/ru/python-net/aspose.cells/validationcollection/copy_to/#int-list-int-int) | Копирует диапазон элементов из списка массивов в совместимый список одномерных массивов, начиная с указанного индекса целевого списка массивов.|
| [index_of(item, index)](/cells/ru/python-net/aspose.cells/validationcollection/index_of/#Validation-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который простирается от указанного индекса до последнего элемента.|
| [index_of(item, index, count)](/cells/ru/python-net/aspose.cells/validationcollection/index_of/#Validation-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который начинается с указанного индекса и содержит указанное количество элементов.|
| [last_index_of(item)](/cells/ru/python-net/aspose.cells/validationcollection/last_index_of/#Validation) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения во всем списке массивов.|
| [last_index_of(item, index)](/cells/ru/python-net/aspose.cells/validationcollection/last_index_of/#Validation-int) |Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который простирается от первого элемента до указанного индекса.|
| [last_index_of(item, index, count)](/cells/ru/python-net/aspose.cells/validationcollection/last_index_of/#Validation-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который содержит указанное количество элементов и заканчивается указанным индексом.|
| [remove_a_cell(row, column)](/cells/ru/python-net/aspose.cells/validationcollection/remove_a_cell/#int-int) | Удаляет все настройки проверки в ячейке.|
| [remove_area(ca)](/cells/ru/python-net/aspose.cells/validationcollection/remove_area/#CellArea) | Удаляет все настройки проверки в диапазоне.|
| [get_validation_in_cell(row, column)](/cells/ru/python-net/aspose.cells/validationcollection/get_validation_in_cell/#int-int) | Получает проверку, применяемую к данной ячейке.|
| [binary_search(item)](/cells/ru/python-net/aspose.cells/validationcollection/binary_search/#Validation) | Ищет элемент во всем отсортированном списке массивов, используя компаратор по умолчанию, и возвращает отсчитываемый от нуля индекс элемента.|



###  Пример

```python
from aspose.cells import CellArea, ValidationType, Workbook

workbook = Workbook()
validations = workbook.worksheets[0].validations
area = CellArea.create_cell_area(0, 0, 1, 1)
validation = validations[validations.add(area)]
validation.type = ValidationType.LIST
validation.formula1 = "a,b,c,d"

```

###  Смотрите также
* модуль [aspose.cells](..)
