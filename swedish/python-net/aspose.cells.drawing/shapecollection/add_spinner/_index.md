---
title: add_spinner metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 290
url: /sv/python-net/aspose.cells.drawing/shapecollection/add_spinner/
is_root: false
---
##  add_spinner(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Lägger till en Spinner i arbetsbladet.


###  Returnerar

Ett Spinner-objekt.


```python
def add_spinner(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| upper_left_row | int | Övre vänstra radens index.|
| top | int |Representerar den vertikala förskjutningen av Spinner från dess vänstra rad, i pixelenhet.|
| upper_left_column | int | Övre vänstra kolumnindex.|
| left | int | Representerar den horisontella förskjutningen av Spinner från dess vänstra kolumn, i pixelenhet.|
| height | int | Representerar höjden på Spinner, i pixelenhet.|
| width | int | Representerar bredden på Spinner, i pixelenhet.|

###  Exempel

```python

# add a spinner
spinner = shapes.add_spinner(1, 0, 1, 0, 100, 50)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)
