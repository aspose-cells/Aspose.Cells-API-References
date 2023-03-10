---
title: add_auto_shape metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 40
url: /sv/python-net/aspose.cells.drawing/shapecollection/add_auto_shape/
is_root: false
---
##  add_auto_shape(type, upper_left_row, top, upper_left_column, left, height, width) {#AutoShapeType-int-int-int-int-int-int}
Lägger till en AutoShape i kalkylbladet.


###  Returnerar

Ett Shape-objekt.


```python
def add_auto_shape(self, type, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| type | [AutoShapeType](/cells/sv/python-net/aspose.cells.drawing/autoshapetype) | Automatisk formtyp.|
| upper_left_row | int | Övre vänstra radens index.|
| top | int | Representerar den vertikala förskjutningen av Shape från dess vänstra rad, i pixelenhet.|
| upper_left_column | int | Övre vänstra kolumnindex.|
| left | int | Representerar den horisontella förskjutningen av Shape från dess vänstra kolumn, i pixelenhet.|
| height | int | Representerar höjden på Shape, i pixelenhet.|
| width | int | Representerar bredden på Shape, i pixelenhet.|
###  Anmärkningar

Typen kunde inte vara Chart/Comment/Picture/OleObject/Polygon/DialogBox
###  Exempel


```python
from aspose.cells.drawing import AutoShapeType

# Adds a AutoShape to the worksheet.
autoShape = shapes.add_auto_shape(AutoShapeType.CUBE, 1, 0, 1, 0, 100, 50)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)
