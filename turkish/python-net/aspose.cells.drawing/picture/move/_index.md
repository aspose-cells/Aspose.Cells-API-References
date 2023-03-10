---
title: move yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 150
url: /tr/python-net/aspose.cells.drawing/picture/move/
is_root: false
---
##  move(upper_left_row, upper_left_column) {#int-int}
Resmi belirtilen bir konuma taşır.



```python
def move(self, upper_left_row, upper_left_column):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| upper_left_row | int | Sol üst sıra dizini.|
| upper_left_column | int | Sol üst sütun dizini.|

###  Örnek

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



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [Picture](/cells/tr/python-net/aspose.cells.drawing/picture)
