---
title: add_check_box metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 70
url: /sv/python-net/aspose.cells.drawing/shapecollection/add_check_box/
is_root: false
---
##  add_check_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Lägger till en kryssruta i kalkylbladet.


###  Returnerar

Det nya CheckBox-objektindexet.


```python
def add_check_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| upper_left_row | int | Övre vänstra radens index.|
| top | int |Representerar den vertikala förskjutningen av kryssrutan från dess vänstra rad, i pixelenhet.|
| upper_left_column | int | Övre vänstra kolumnindex.|
| left | int | Representerar den horisontella förskjutningen av textrutan från dess vänstra kolumn, i pixelenhet.|
| height | int | Textrutans höjd, i pixelenhet.|
| width | int | Textrutans bredd, i pixelenhet.|

###  Exempel

```python

# add a CheckBox
checkBox = shapes.add_check_box(1, 0, 1, 0, 100, 50)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)
