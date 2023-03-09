---
title: move метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 150
url: /ru/python-net/aspose.cells.drawing/picture/move/
is_root: false
---
##  move(upper_left_row, upper_left_column) {#int-int}
Перемещает изображение в указанное место.



```python
def move(self, upper_left_row, upper_left_column):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| upper_left_column | int |Индекс левого верхнего столбца.|

###  Пример

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
imgIndex = worksheet.pictures.add(1, 1, "example.jpeg")
# Get the inserted picture object
pic = worksheet.pictures[imgIndex]
# Set the new location of the picture
pic.move(2, 4)
# Save the excel file.
workbook.save("result.xlsx")

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [Picture](/cells/ru/python-net/aspose.cells.drawing/picture)
