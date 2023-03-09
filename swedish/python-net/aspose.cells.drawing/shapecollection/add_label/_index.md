---
title: add_label metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 130
url: /sv/python-net/aspose.cells.drawing/shapecollection/add_label/
is_root: false
---
##  add_label(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Lägger till en etikett i kalkylbladet.


###  Returnerar

Ett etikettobjekt.


```python
def add_label(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| upper_left_row | int | Övre vänstra radens index.|
| top | int | Representerar den vertikala förskjutningen av etiketten från dess vänstra rad, i pixelenhet.|
| upper_left_column | int |Övre vänstra kolumnindex.|
| left | int | Representerar den horisontella förskjutningen av etiketten från dess vänstra kolumn, i pixelenhet.|
| height | int | Representerar höjden på etiketten i pixelenhet.|
| width | int | Representerar etikettens bredd i pixelenhet.|

###  Exempel

```python

# add a label
label = shapes.add_label(1, 0, 1, 0, 100, 50)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)
