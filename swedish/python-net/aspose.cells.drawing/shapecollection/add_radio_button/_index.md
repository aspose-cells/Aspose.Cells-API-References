---
title: add_radio_button metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 230
url: /sv/python-net/aspose.cells.drawing/shapecollection/add_radio_button/
is_root: false
---
##  add_radio_button(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Lägger till en RadioButton i arbetsbladet.


###  Returnerar

Ett RadioButton-objekt.


```python
def add_radio_button(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| upper_left_row | int | Övre vänstra radens index.|
| top | int | Representerar den vertikala förskjutningen av RadioButton från dess vänstra rad, i pixelenhet.|
| upper_left_column | int |Övre vänstra kolumnindex.|
| left | int | Representerar den horisontella förskjutningen av RadioButton från dess vänstra kolumn, i pixelenhet.|
| height | int |Representerar höjden på RadioButton, i pixelenhet.|
| width | int | Representerar bredden på RadioButton, i pixelenhet.|

###  Exempel

```python

# add a radio button
radioButton = shapes.add_radio_button(1, 0, 1, 0, 100, 50)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)
