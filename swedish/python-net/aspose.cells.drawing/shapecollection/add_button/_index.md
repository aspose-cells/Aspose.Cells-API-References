---
title: add_button metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 60
url: /sv/python-net/aspose.cells.drawing/shapecollection/add_button/
is_root: false
---
##  add_button(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Lägger till en knapp i kalkylbladet.


###  Returnerar

Ett knappobjekt.


```python
def add_button(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| upper_left_row | int | Övre vänstra radens index.|
| top | int | Representerar den vertikala förskjutningen av knappen från dess vänstra rad, i pixelenhet.|
| upper_left_column | int | Övre vänstra kolumnindex.|
| left | int | Representerar den horisontella förskjutningen av knappen från dess vänstra kolumn, i pixelenhet.|
| height | int | Representerar höjden på knappen, i pixelenhet.|
| width | int | Representerar knappens bredd i pixelenhet.|

###  Exempel

```python

# add a button
button = shapes.add_button(1, 0, 1, 0, 100, 50)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)
