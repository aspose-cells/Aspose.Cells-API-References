---
title: add_rectangle metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 240
url: /sv/python-net/aspose.cells.drawing/shapecollection/add_rectangle/
is_root: false
---
##  add_rectangle(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Lägger till en RectangleShape till kalkylbladet.


###  Returnerar

Ett RectangleShape-objekt.


```python
def add_rectangle(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| upper_left_row | int | Övre vänstra radens index.|
| top | int | Representerar den vertikala förskjutningen av RectangleShape från dess vänstra rad, i pixelenhet.|
| upper_left_column | int |Övre vänstra kolumnindex.|
| left | int | Representerar den horisontella förskjutningen av RectangleShape från dess vänstra kolumn, i pixelenhet.|
| height | int | Representerar höjden på RectangleShape, i pixelenhet.|
| width | int | Representerar bredden på RectangleShape, i pixelenhet.|

###  Exempel

```python

#  add a rectangle
rectangleShape = shapes.add_rectangle(2, 0, 2, 0, 130, 130)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)
