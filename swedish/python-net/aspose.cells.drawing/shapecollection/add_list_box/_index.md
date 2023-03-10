---
title: add_list_box metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 170
url: /sv/python-net/aspose.cells.drawing/shapecollection/add_list_box/
is_root: false
---
##  add_list_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Lägger till en ListBox i kalkylbladet.


###  Returnerar

Ett ListBox-objekt.


```python
def add_list_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| upper_left_row | int | Övre vänstra radens index.|
| top | int | Representerar den vertikala förskjutningen av ListBox från dess vänstra rad, i pixelenhet.|
| upper_left_column | int | Övre vänstra kolumnindex.|
| left | int | Representerar den horisontella förskjutningen av ListBox från dess vänstra kolumn, i pixelenhet.|
| height | int | Representerar höjden på ListBox, i pixelenhet.|
| width | int | Representerar bredden på ListBox, i pixelenhet.|

###  Exempel

```python

# add a list box
listBox = shapes.add_list_box(1, 0, 1, 0, 100, 50)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)
