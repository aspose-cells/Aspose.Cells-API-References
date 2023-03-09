---
title: add_oval metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 200
url: /sv/python-net/aspose.cells.drawing/shapecollection/add_oval/
is_root: false
---
##  add_oval(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Lägger till en oval i arbetsbladet.


###  Returnerar

Ett ovalt föremål.


```python
def add_oval(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| upper_left_row | int | Övre vänstra radens index.|
| top | int | Representerar den vertikala förskjutningen av Oval från dess vänstra rad, i pixelenhet.|
| upper_left_column | int |Övre vänstra kolumnindex.|
| left | int | Representerar den horisontella förskjutningen av Oval från dess vänstra kolumn, i pixelenhet.|
| height | int | Representerar höjden på Oval, i pixelenhet.|
| width | int | Representerar bredden på Oval, i pixelenhet.|

###  Exempel

```python

# add a oval
oval = shapes.add_oval(1, 0, 1, 0, 50, 50)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)
