---
title: RowCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 1310
url: /ru/python-net/aspose.cells/rowcollection/
is_root: false
---
##  RowCollection класс
Собирает объекты [Row](/cells/ru/python-net/aspose.cells/row), представляющие отдельные строки на листе.



Тип RowCollection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [count](/cells/ru/python-net/aspose.cells/rowcollection/count) | Получает количество строк в этой коллекции.|



Получает объект [Row](/cells/ru/python-net/aspose.cells/row) по заданному индексу строки. Объект Row с заданным индексом строки будет создан, если он не существовал ранее.
###  Индексатор
| Имя| Описание|
| :- | :- |
| [index] |  |


###  Методы
| Метод| Описание|
| :- | :- |
| [get_row_by_index(index)](/cells/ru/python-net/aspose.cells/rowcollection/get_row_by_index/#int) | Получает объект строки по позиции в списке.|
| [clear()](/cells/ru/python-net/aspose.cells/rowcollection/clear/#) | Очистить все строки и ячейки.|
| [remove_at(index)](/cells/ru/python-net/aspose.cells/rowcollection/remove_at/#int) | Удалить строку по указанному индексу|



###  Пример

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Get first row
row = worksheet.cells.rows[0]

```

###  Смотрите также
* модуль [aspose.cells](..)
* класс [Row](/cells/ru/python-net/aspose.cells/row)
