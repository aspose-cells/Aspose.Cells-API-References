---
title: ColumnCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 270
url: /ru/python-net/aspose.cells/columncollection/
is_root: false
---
##  ColumnCollection класс
Коллекция объектов [Column](/cells/ru/python-net/aspose.cells/column), представляющих отдельные столбцы (параметры) на листе.
Объект Column представляет только такие настройки, как ширина столбца, стили и т. д.
не имеет никакого отношения к тому, что в соответствующих столбцах есть непустые ячейки (данные).
И «Количество» этой коллекции представляет только количество объектов столбца, которые были созданы в этой коллекции,
не имеет ничего общего с тем, что на листе есть непустые ячейки (данные) или нет.



Тип ColumnCollection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [capacity](/cells/ru/python-net/aspose.cells/columncollection/capacity) | Получает или задает количество элементов, которые может содержать список массивов.|


###  Методы
| Метод| Описание|
| :- | :- |
| [copy_to(array)](/cells/ru/python-net/aspose.cells/columncollection/copy_to/#list) | Копирует весь список массивов в совместимый список одномерных массивов, начиная с начала целевого списка массивов.|
| [copy_to(index, array, array_index, count)](/cells/ru/python-net/aspose.cells/columncollection/copy_to/#int-list-int-int) |Копирует диапазон элементов из списка массивов в совместимый список одномерных массивов, начиная с указанного индекса целевого списка массивов.|
| [index_of(item, index)](/cells/ru/python-net/aspose.cells/columncollection/index_of/#Column-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который простирается от указанного индекса до последнего элемента.|
| [index_of(item, index, count)](/cells/ru/python-net/aspose.cells/columncollection/index_of/#Column-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который начинается с указанного индекса и содержит указанное количество элементов.|
| [last_index_of(item)](/cells/ru/python-net/aspose.cells/columncollection/last_index_of/#Column) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения во всем списке массивов.|
| [last_index_of(item, index)](/cells/ru/python-net/aspose.cells/columncollection/last_index_of/#Column-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который простирается от первого элемента до указанного индекса.|
| [last_index_of(item, index, count)](/cells/ru/python-net/aspose.cells/columncollection/last_index_of/#Column-int-int) |Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который содержит указанное количество элементов и заканчивается указанным индексом.|
| [get_by_index(index)](/cells/ru/python-net/aspose.cells/columncollection/get_by_index/#int) | Получает объект столбца по индексу.|
| [get_column_by_index(index)](/cells/ru/python-net/aspose.cells/columncollection/get_column_by_index/#int) | Получает объект [Column](/cells/ru/python-net/aspose.cells/column) по позиции в списке.|
| [binary_search(item)](/cells/ru/python-net/aspose.cells/columncollection/binary_search/#Column) | Ищет элемент во всем отсортированном списке массивов, используя компаратор по умолчанию, и возвращает отсчитываемый от нуля индекс элемента.|



###  Примеры

```python
from aspose.cells import BackgroundType, StyleFlag, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Add new Style to Workbook
style = workbook.create_style()
# Setting the background color to Blue
style.foreground_color = Color.blue
# setting Background Pattern
style.pattern = BackgroundType.SOLID
# New Style Flag
styleFlag = StyleFlag()
# Set All Styles
styleFlag.all = True
# Change the default width of first ten columns
for i in range(10):
    worksheet.cells.columns[i].width = 20
# Get the Column with non default formatting
columns = worksheet.cells.columns
for column in columns:
    # Apply Style to first ten Columns
    column.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  Смотрите также
* модуль [aspose.cells](..)
* класс [Column](/cells/ru/python-net/aspose.cells/column)
