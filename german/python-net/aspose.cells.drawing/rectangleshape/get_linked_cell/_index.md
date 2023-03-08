---
title: get_linked_cell Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 100
url: /de/python-net/aspose.cells.drawing/rectangleshape/get_linked_cell/
is_root: false
---
##  get_linked_cell(is_r1c1, is_local) {#bool-bool}
Ruft den Bereich ab, der mit dem Wert des Steuerelements verknüpft ist.


###  Kehrt zurück

Der Bereich, der mit dem Wert des Steuerelements verknüpft ist.


```python
def get_linked_cell(self, is_r1c1, is_local):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| is_r1c1 | bool | Ob die Formel als R1C1 formatiert werden muss.|
| is_local | bool | Ob die Formel nach Gebietsschema formatiert werden muss.|

###  Beispiel

```python

# You may get results like '$A$1'
link = shape.get_linked_cell(False, False)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [RectangleShape](/cells/de/python-net/aspose.cells.drawing/rectangleshape)
