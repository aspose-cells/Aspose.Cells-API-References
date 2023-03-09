---
title: add_shape metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 260
url: /sv/python-net/aspose.cells.drawing/shapecollection/add_shape/
is_root: false
---
##  add_shape(type, upper_left_row, top, upper_left_column, left, height, width) {#MsoDrawingType-int-int-int-int-int-int}
Lägger till en form i kalkylbladet.


###  Returnerar

Ett Shape-objekt.


```python
def add_shape(self, type, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| type | [MsoDrawingType](/cells/sv/python-net/aspose.cells.drawing/msodrawingtype) | Mso ritningstyp.|
| upper_left_row | int | Övre vänstra radens index.|
| top | int | Representerar den vertikala förskjutningen av Shape från dess vänstra rad, i pixelenhet.|
| upper_left_column | int | Övre vänstra kolumnindex.|
| left | int | Representerar den horisontella förskjutningen av Shape från dess vänstra kolumn, i pixelenhet.|
| height | int | Representerar höjden på Shape, i enheter av pixlar.|
| width | int | Representerar bredden på Shape, i enheter av pixlar.|
###  Anmärkningar

Typen kunde inte vara Chart/Comment/Picture/OleObject/Polygon/DialogBox
###  Exempel


```python
from aspose.cells.drawing import MsoDrawingType

# Add a shape of the specified type
shapeByType = shapes.add_shape(MsoDrawingType.CELLS_DRAWING, 1, 0, 1, 0, 100, 50)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)
