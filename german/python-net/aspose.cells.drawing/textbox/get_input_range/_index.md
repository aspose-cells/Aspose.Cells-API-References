---
title: get_input_range Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 90
url: /de/python-net/aspose.cells.drawing/textbox/get_input_range/
is_root: false
---
##  get_input_range(is_r1c1, is_local) {#bool-bool}
Ruft den Bereich ab, der zum Füllen des Steuerelements verwendet wird.


###  Kehrt zurück

Der zum Füllen des Steuerelements verwendete Bereich.


```python
def get_input_range(self, is_r1c1, is_local):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| is_r1c1 | bool | Ob die Formel als R1C1 formatiert werden muss.|
| is_local | bool | Ob die Formel nach Gebietsschema formatiert werden muss.|

###  Beispiel

```python

range = shape.get_input_range(False, True)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [TextBox](/cells/de/python-net/aspose.cells.drawing/textbox)
