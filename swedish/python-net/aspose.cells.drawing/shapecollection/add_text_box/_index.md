---
title: add_text_box metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 310
url: /sv/python-net/aspose.cells.drawing/shapecollection/add_text_box/
is_root: false
---
##  add_text_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Lägger till en textruta i kalkylbladet.


###  Returnerar

Ett [TextBox](/cells/sv/python-net/aspose.cells.drawing/textbox) objekt.


```python
def add_text_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| upper_left_row | int | Övre vänstra radens index.|
| top | int |Representerar den vertikala förskjutningen av textrutan från dess vänstra rad, i pixelenhet.|
| upper_left_column | int |Övre vänstra kolumnindex.|
| left | int | Representerar den horisontella förskjutningen av textrutan från dess vänstra kolumn, i pixelenhet.|
| height | int | Representerar höjden på textrutan, i pixelenhet.|
| width | int | Representerar bredden på textrutan, i pixelenhet.|

###  Exempel

```python

# add a TextBox
textBox = shapes.add_text_box(1, 0, 1, 0, 100, 50)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)
* klass [TextBox](/cells/sv/python-net/aspose.cells.drawing/textbox)
