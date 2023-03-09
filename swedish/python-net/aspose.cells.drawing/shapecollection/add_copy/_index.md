---
title: add_copy metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 90
url: /sv/python-net/aspose.cells.drawing/shapecollection/add_copy/
is_root: false
---
##  add_copy(source_shape, upper_left_row, top, upper_left_column, left) {#Shape-int-int-int-int}
Lägger till och kopierar en form till kalkylbladet.


###  Returnerar

Det nya formobjektindexet.


```python
def add_copy(self, source_shape, upper_left_row, top, upper_left_column, left):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| source_shape | [Shape](/cells/sv/python-net/aspose.cells.drawing/shape) | Källform.|
| upper_left_row | int | Övre vänstra radens index.|
| top | int | Representerar den vertikala förskjutningen av kryssrutan från dess vänstra rad, i pixelenhet.|
| upper_left_column | int |Övre vänstra kolumnindex.|
| left | int | Representerar den horisontella förskjutningen av textrutan från dess vänstra kolumn, i pixelenhet.|

###  Exempel

```python

# add a shape
rectangle = shapes.add_rectangle(2, 0, 2, 0, 130, 130)
# copy
shapes.add_copy(rectangle, 7, 0, 7, 0)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)
