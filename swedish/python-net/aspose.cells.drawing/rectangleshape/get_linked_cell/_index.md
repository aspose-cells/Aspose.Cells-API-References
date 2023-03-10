---
title: get_linked_cell metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 100
url: /sv/python-net/aspose.cells.drawing/rectangleshape/get_linked_cell/
is_root: false
---
##  get_linked_cell(is_r1c1, is_local) {#bool-bool}
Får intervallet kopplat till kontrollens värde.


###  Returnerar

Området kopplat till kontrollens värde.


```python
def get_linked_cell(self, is_r1c1, is_local):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| is_r1c1 | bool | Om formeln behöver formateras som R1C1.|
| is_local | bool | Huruvida formeln behöver formateras efter språk.|

###  Exempel

```python

# You may get results like '$A$1'
link = shape.get_linked_cell(False, False)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [RectangleShape](/cells/sv/python-net/aspose.cells.drawing/rectangleshape)
