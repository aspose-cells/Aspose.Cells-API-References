---
title: add_line metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 150
url: /sv/python-net/aspose.cells.drawing/shapecollection/add_line/
is_root: false
---
##  add_line(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Lägger till en LineShape i kalkylbladet.


###  Returnerar

Ett LineShape-objekt.


```python
def add_line(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| upper_left_row | int | Övre vänstra radens index.|
| top | int | Representerar den vertikala förskjutningen av LineShape från dess vänstra rad, i pixelenhet.|
| upper_left_column | int |Övre vänstra kolumnindex.|
| left | int | Representerar den horisontella förskjutningen av LineShape från dess vänstra kolumn, i pixelenhet.|
| height | int | Representerar höjden på LineShape, i pixelenhet.|
| width | int | Representerar bredden på LineShape, i pixelenhet.|

###  Exempel

```python

#  add a line object
lineShape = shapes.add_line(1, 0, 1, 0, 100, 50)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)
